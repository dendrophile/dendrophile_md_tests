GUI Basics
==========


This section will explain the bare necessities for scripting <span class=keyword>Controls</span> with <span class=keyword>UnityGUI</span>.

Making Controls with UnityGUI
-----------------------------


UnityGUI controls make use of a special function called <span class=component>OnGUI()</span>.  The <span class=component>OnGUI()</span> function gets called every frame as long as the containing script is enabled - just like the <span class=component>Update()</span> function.

GUI controls themselves are very simple in structure.  This structure is evident in the following example.

````

/* Example level loader */


// JavaScript
function OnGUI () {
	// Make a background box
	GUI.Box (Rect (10,10,100,90), "Loader Menu");

	// Make the first button. If it is pressed, Application.Loadlevel (1) will be executed
	if (GUI.Button (Rect (20,40,80,20), "Level 1")) {
		Application.LoadLevel (1);
	}

	// Make the second button.
	if (GUI.Button (Rect (20,70,80,20), "Level 2")) {
		Application.LoadLevel (2);
	}
}


//C#
using UnityEngine;
using System.Collections;

public class GUITest : MonoBehaviour {
			
	void OnGUI () {
		// Make a background box
		GUI.Box(new Rect(10,10,100,90), "Loader Menu");
	
		// Make the first button. If it is pressed, Application.Loadlevel (1) will be executed
		if(GUI.Button(new Rect(20,40,80,20), "Level 1")) {
			Application.LoadLevel(1);
		}
	
		// Make the second button.
		if(GUI.Button(new Rect(20,70,80,20), "Level 2")) {
			Application.LoadLevel(2);
		}
	}
}

````

This example is a complete, functional level loader. If you copy/paste this script and attach it a <span class=keyword>GameObject</span>, you'll see the following menu appear in when you enter <span class=keyword>Play Mode</span>:


![](http://docwiki.hq.unity3d.com/uploads/Main/guiScripting-BasicsLoaderMenuExample.png)  
_The Loader Menu created by the example code_

Let's take a look at the details of the example code:

The first GUI line, <span class=component>GUI.Box (Rect (10,10,100,90), "Loader Menu");</span> displays a <span class=keyword>Box</span> Control with the header text "Loader Menu".  It follows the typical GUI Control declaration scheme which we'll explore momentarily.

The next GUI line is a <span class=keyword>Button</span> Control declaration.  Notice that it is slightly different from the Box Control declaration.  Specifically, the entire Button declaration is placed inside an <span class=component>if</span> statement.  When the game is running and the Button is clicked, this <span class=component>if</span> statement returns true and any code inside the <span class=component>if</span> block is executed.

Since the <span class=component>OnGUI()</span> code gets called every frame, you don't need to explicitly create or destroy GUI controls. The line that declares the Control is the same one that creates it.  If you need to display Controls at specific times, you can use any kind of scripting logic to do so.

````

/* Flashing button example */


// JavaScript
function OnGUI () {
	if (Time.time % 2 < 1) {
		if (GUI.Button (Rect (10,10,200,20), "Meet the flashing button")) {
			print ("You clicked me!");
		}
	}
}


// C#
using UnityEngine;
using System.Collections;

public class GUITest : MonoBehaviour {
			
	void OnGUI () {
		if (Time.time % 2 < 1) {
			if (GUI.Button (new Rect (10,10,200,20), "Meet the flashing button")) {
				print ("You clicked me!");
			}
		}
	}
}

````

Here, <span class=component>GUI.Button()</span> only gets called every other second, so the button will appear and disappear. Naturally, the user can only click it when the button is visible.

As you can see, you can use any desired logic to control when GUI Controls are displayed and functional.  Now we will explore the details of each Control's declaration.


Anatomy of a Control
--------------------


There are three key pieces of information required when declaring a GUI Control:

<span class=keyword>Type</span> (<span class=keyword>Position</span>, <span class=keyword>Content</span>)

Observe that this structure is a function with two arguments.  We'll explore the details of this structure now.


###Type

<span class=keyword>Type</span> is the <span class=keyword>Control Type</span>, and is declared by calling a function in Unity's [GUI class](ScriptRef:GUI.html) or the [GUILayout class](ScriptRef:GUILayout.html), which is discussed at length in the [Layout Modes](gui-Layout.md) section of the Guide.  For example, <span class=component>GUI.Label()</span> will create a non-interactive label.  All the different control types are explained later, in the [Controls](gui-Controls.md) section of the Guide.


###Position

The <span class=keyword>Position</span> is the first argument in any <span class=component>GUI</span> Control function.  The argument itself is provided with a <span class=component>Rect()</span> function.  <span class=component>Rect()</span> defines four properties: <span class=keyword>left-most position</span>, <span class=keyword>top-most position</span>, <span class=keyword>total width</span>, <span class=keyword>total height</span>.  All of these values are provided in <span class=keyword>integers</span>, which correspond to pixel values.  All UnityGUI controls work in <span class=keyword>Screen Space</span>, which is the resolution of the published player in pixels.

The coordinate system is top-left based.  <span class=component>Rect(10, 20, 300, 100)</span> defines a Rectangle that starts at coordinates: 10,20  and ends at coordinates 310,120.  It is worth repeating that the second pair of values in <span class=component>Rect()</span> are total width and height, not the coordinates where the controls end.  This is why the example mentioned above ends at 310,120 and not 300,100.

You can use the <span class=component>Screen.width</span> and <span class=component>Screen.height</span> properties to get the total dimensions of the screen space available in the player.  The following example may help clarify how this is done:

````

/* Screen.width & Screen.height example */


// JavaScript
function OnGUI () {
	GUI.Box (Rect (0,0,100,50), "Top-left");
	GUI.Box (Rect (Screen.width - 100,0,100,50), "Top-right");
	GUI.Box (Rect (0,Screen.height - 50,100,50), "Bottom-left");
	GUI.Box (Rect (Screen.width - 100,Screen.height - 50,100,50), "Bottom-right");
}


// C#
using UnityEngine;
using System.Collections;

public class GUITest : MonoBehaviour {
			
	void OnGUI(){
		GUI.Box (new Rect (0,0,100,50), "Top-left");
		GUI.Box (new Rect (Screen.width - 100,0,100,50), "Top-right");
		GUI.Box (new Rect (0,Screen.height - 50,100,50), "Bottom-left");
		GUI.Box (new Rect (Screen.width - 100,Screen.height - 50,100,50), "Bottom-right");
	}

}

````


![](http://docwiki.hq.unity3d.com/uploads/Main/gsg-ScreenWidthHeight.png)  
_The Boxes positioned by the above example_


###Content

The second argument for a GUI Control is the actual content to be displayed with the Control.  Most often you will want to display some text or an image on your Control.  To display text, pass a string as the Content argument like this:

````

/* String Content example */


// JavaScript
function OnGUI () {
	GUI.Label (Rect (0,0,100,50), "This is the text string for a Label Control");
}


// C#
using UnityEngine;
using System.Collections;

public class GUITest : MonoBehaviour {
			
	void OnGUI () {
		GUI.Label (new Rect (0,0,100,50), "This is the text string for a Label Control");
	}

}

````

To display an image, declare a <span class=keyword>Texture2D</span> public variable, and pass the variable name as the content argument like this:

````

/* Texture2D Content example */


// JavaScript
var controlTexture : Texture2D;

function OnGUI () {
	GUI.Label (Rect (0,0,100,50), controlTexture);
}


// C#
public Texture2D controlTexture;
  ...

void OnGUI () {
	GUI.Label (new Rect (0,0,100,50), controlTexture);
}

````

Here is an example closer to a real-world scenario:

````

/* Button Content examples */


// JavaScript
var icon : Texture2D;

function OnGUI () {
	if (GUI.Button (Rect (10,10, 100, 50), icon)) {
		print ("you clicked the icon");
	}

	if (GUI.Button (Rect (10,70, 100, 20), "This is text")) {
		print ("you clicked the text button");
	}
}


// C#
using UnityEngine;
using System.Collections;

public class GUITest : MonoBehaviour {
				
	public Texture2D icon;
	
	void OnGUI () {
		if (GUI.Button (new Rect (10,10, 100, 50), icon)) {
			print ("you clicked the icon");
		}
	
		if (GUI.Button (new Rect (10,70, 100, 20), "This is text")) {
			print ("you clicked the text button");
		}
	}

}

````


![](http://docwiki.hq.unity3d.com/uploads/Main/gsg-IconStringContent.png)  
_The Buttons created by the above example_

There is a third option which allows you to display images and text together in a GUI Control.  You can provide a <span class=keyword>GUIContent</span> object as the Content argument, and define the string and image to be displayed within the GUIContent.

````

/* Using GUIContent to display an image and a string */


// JavaScript
var icon : Texture2D;

function OnGUI () {
	GUI.Box (Rect (10,10,100,50), GUIContent("This is text", icon));
}


// C#
using UnityEngine;
using System.Collections;

public class GUITest : MonoBehaviour {
				
	public Texture2D icon;

	void OnGUI () {
		GUI.Box (new Rect (10,10,100,50), new GUIContent("This is text", icon));
	}

}

````

You can also define a <span class=keyword>Tooltip</span> in the GUIContent, and display it elsewhere in the GUI when the mouse hovers over it.

````

/* Using GUIContent to display a tooltip */


// JavaScript
function OnGUI () {
	// This line feeds "This is the tooltip" into GUI.tooltip
	GUI.Button (Rect (10,10,100,20), GUIContent ("Click me", "This is the tooltip"));
	// This line reads and displays the contents of GUI.tooltip
	GUI.Label (Rect (10,40,100,20), GUI.tooltip);
}


// C#
using UnityEngine;
using System.Collections;

public class GUITest : MonoBehaviour {
					
	void OnGUI () {
		// This line feeds "This is the tooltip" into GUI.tooltip
		GUI.Button (new Rect (10,10,100,20), new GUIContent ("Click me", "This is the tooltip"));
		
		// This line reads and displays the contents of GUI.tooltip
		GUI.Label (new Rect (10,40,100,20), GUI.tooltip);
	}

}

````


If you're daring you can also use GUIContent to display a string, an icon, and a tooltip! 

````

/* Using GUIContent to display an image, a string, and a tooltip */


// JavaScript
var icon : Texture2D;

function OnGUI () {
	GUI.Button (Rect (10,10,100,20), GUIContent ("Click me", icon, "This is the tooltip"));
	GUI.Label (Rect (10,40,100,20), GUI.tooltip);
}


// C#
using UnityEngine;
using System.Collections;

public class GUITest : MonoBehaviour {
					
	public Texture2D icon;
	
	void OnGUI () {
		GUI.Button (new Rect (10,10,100,20), new GUIContent ("Click me", icon, "This is the tooltip"));
		GUI.Label (new Rect (10,40,100,20), GUI.tooltip);
	}

}

````

The scripting reference page for [GUIContent's constructor](ScriptRef:GUIContent.GUIContent.html) for an extensive list of examples.
