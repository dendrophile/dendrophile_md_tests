AssetBundles (Pro only)
=======================


AssetBundles are files which you can export from Unity to contain assets of your choice. These files use a proprietary compressed format and can be loaded on demand by your application. This allows you to stream in content, such as models, textures, audio clips, or even entire scenes separately from the scene in which they will be used. AssetBundles have been designed to simplify downloading content to your application.
AssetBundles can contain any kind of asset type recognized by Unity, as determined by the filename extension. If you want to include files with custom binary data, they should have the extension ".bytes". Unity will import these files as TextAssets.

When working with AssetBundles, here's the typical workflow:

_During development_, the developer prepares AssetBundles and uploads them to a server.
![](http://docwiki.hq.unity3d.com/uploads/Main/AssetBundlesBuildPlusUpload.jpg)  
                       Building and uploading asset bundles

1. __Building AssetBundles__. Asset bundles are created in the editor from assets in your scene. The Asset Bundle building process is described in more detail in the section for [Building AssetBundles](buildingassetbundles.html)

1. __Uploading AssetBundles to external storage__. This step does not include the Unity Editor or any other Unity channels, but we include it for completeness. You can use an [FTP client](http://en.wikipedia.org/wiki/file_transfer_protocol.html) to upload your Asset Bundles to the server of your choice.


_At runtime_, on the user's machine, the application will load AssetBundles on demand and operate individual assets within each AssetBundle as needed. 
![](http://docwiki.hq.unity3d.com/uploads/Main/AssetBundlesDownloadPlusLoad.jpg)  
                       Downloading AssetBundles and loading assets from them

1. __Downloading AssetBundles at runtime from your application__. This is done from script within a Unity scene, and Asset Bundles are loaded from the server on demand. More on that in [Downloading Asset Bundles](downloadingassetbundles.html).

1. __Loading objects from AssetBundles__. Once the AssetBundle is downloaded, you might want to access its individual Assets from the Bundle. More on that in [Loading Resources from AssetBundles](loadingassetbundles.html)


See also:
* [Frequently Asked Questions](abfaq.html)
* [Building AssetBundles](buildingassetbundles.html)
* [Downloading Asset Bundles](downloadingassetbundles.html)
* [Loading Asset Bundles](loadingassetbundles.html)
* [Keeping track of loaded AssetBundles](keepingtrackofloadedassetbundles.html)
* [Storing and loading binary data](binarydata.html)
* [Protecting content](protectingcontent.html)
* [Managing Asset Dependencies](managingassetdependencies.html)
* [Including scripts in AssetBundles](scriptsinassetbundles.html)
