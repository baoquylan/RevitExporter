# RvtVa3c

A Revit custom exporter add-in generating JSON output for the [vA3C](http://va3c.github.io) [three.js](http://threejs.org) AEC viewer.


## Setup, Compilation and Installation

RvtVa3c is a Revit add-in implementing an external application and an external command.

It is installed in the standard manner, i.e., by copying two files to the standard Revit Add-Ins folder:

- The .NET assembly DLL `RvtVa3c.dll`
- The add-in manifest `RvtVa3c.addin`

In order to generate the DLL, you download and compile the Visual Studio solution:

- Download or clone the [RvtVa3c GitHub repository](https://github.com/va3c/RvtVa3c).
- Open the solution file RvtVa3c.sln in Visual Studio; to build it:
- Add references to the Revit API assembly files `RevitAPI.dll` and `RevitAPIUI.dll`, located in your Revit installation directory.
- If you wish to debug, set up the path to the Revit executable in the Debug tab, Start External Program; change the path to your system installation, e.g., `C:\Program Files\Autodesk\Revit Architecture 2017\Revit.exe`.
- Build and optionally debug into Revit.exe.

This will open the Revit installation and install the plugin.

You can then either start up Revit.exe manually or via the Visual Studio debugger.

In Revit, the RvtVa3c add-in external command can be launched from the Revit Add-Ins tab, which causes it to export your Revit model to a JSON file.

For more information on setting up Revit to discover and load the add-in, please refer to 
the [Revit online help](http://help.autodesk.com/view/RVT/2017/ENU) &gt; Developers 
&gt; [Revit API Developers Guide](http://help.autodesk.com/view/RVT/2017/ENU/?guid=GUID-F0A122E0-E556-4D0D-9D0F-7E72A9315A42) 
&gt; [Introduction](http://help.autodesk.com/cloudhelp/2017/ENU/Revit-API/files/GUID-C574D4C8-B6D2-4E45-93A5-7E35B7E289BE.htm) 
&gt; [Add-In Integration](http://help.autodesk.com/cloudhelp/2017/ENU/Revit-API/files/GUID-4BE74935-A15C-4536-BD9C-7778766CE392.htm) 
&gt; [Add-in Registration](http://help.autodesk.com/cloudhelp/2017/ENU/Revit-API/files/GUID-4FFDB03E-6936-417C-9772-8FC258A261F7.htm).

For more details on programming Revit add-ins in general, please refer to the [Revit API Getting Started](http://thebuildingcoder.typepad.com/blog/about-the-author.html#2) material, especially the DevTV and My First Revit Plugin tutorials.

![alt text](https://github.com/baoquylan/RvtVa3c/blob/master/image/demo.gif?raw=true)

## Tools and Technologies

* [three.js JavaScript 3D Library](https://github.com/mrdoob/three.js)
* [vA3C three.js AEC Viewer](http://va3c.github.io)

## New

* Updated for Threejs version >= 125
* Add texture for exporter
* Change dimension from millimeters to meters

## Wishlist

* Export to GLTF

## Authors

Updated and maintained by LanBao

## About

The project inspired by [RvtVa3C](https://github.com/va3c/RvtVa3c) and was forked for research purpose


## <a name="license"></a>License

This sample is licensed under the terms of the [MIT License](http://opensource.org/licenses/MIT).
Please see the [LICENSE](LICENSE) file for full details.

