# OD_CopyPasteExternal
Easily copying and pasting of geometry between 3D Applications              [Quick Download](https://github.com/heimlich1024/OD_CopyPasteExternal/archive/master.zip)

# Why ?

Because quite frankly nothing thats this easy exists.  And if you are like me working in environments using
multiple applications, this becomes extremely beneficial.  I opensourced it, in the hope, that there are other
people willing to contributes, in applications that I have either a) not touched, or b) have not as much experience
in to make this even better than it already is.  So if you are willing to contribute, please get in touch with me.

Currently, it uses an always existing temporary directory to store the intermediate custom file on the local machine,
but of course that directory can be changed to live on a dropbox (for online internet sharing with friends), or on a
network server for inter company sharing.  Those are really just some of the possibilies.

# Help ?

If you want to help and contribute, please get in touch with me.  There's XSI, Cinema4D and 3dsMax that still need
to be done, as well as the Houdini Exporter.  So anyone with experience in the SDK on those apps, please take a look.

# General Information:

* Copy To External: will copy the current mesh into memory
* Paste From External: will rebuild the geometry thats in memory

The following applications are supported:

* Modo      : Vertices / Polygons (incl. Subpatch and SubD)/ WeightMaps / UVMaps / MorphMaps
* Lightwave : Vertices / Polygons (incl. Subpatch and SubD)/ WeightMaps / UVMaps / MorphMaps
* Blender   : Vertices / Polygons (incl. Subpatch and SubD)/ WeightMaps / UVMaps / MorphMaps
* Maya      : Vertices / Polygons / Weights (via Vertex Normals) (Implementation by Andre Hotz)
* Houdini   : Vertices / Polygons / Weightmaps, UVMaps (Paste Implementation by Chris Wells)
* Others	: Looking for contributors to write implementations for other 3d Apps (see TODO)

# Installation:

### MODO Install (tested 10.01 and higher):

Drag the OD_ModoCopyPasteExternal folder into your kits folder.
Upon Modo start/restart you now have two additional commands:

OD_CopyToExternal & OD_PasteFromExternal

You'll see a Scissors Icon in your Tailbar which includes those commands.

### LIGHTWAVE Install (2015+):

Add the LW_CopyPasteExternal.py via add plugins. 3 Plugins should be added:

in Layout: OD_LayoutPasteFromExternal
in Modeler: OD_LWPasteFromExternal & OD_LWCopyToExternal
Add them to the menus as you please.

### Maya Install

Just install the two scripts as any other plugin.

### Blender Install (tested 2.78c)

Preferences/Addons/Install from File and select the files and click the checkbox.
The plugins are then found under the object menu.

### Houdini Install (tested 15 and higher)

Start Houdini and Right Click on an empty space in the shelf and select New Tool.
Then go to the Scrips Tab and paste the contents of the python file there.  In the
options tab, you can name the tools, click apply and accept, and you are good to go.


# Tutorials & Videos

Steve White has provided a Youtube Video here showing the use between Modo and Lightwave.

<a href="http://www.youtube.com/watch?feature=player_embedded&v=6jKi34irylo
" target="_blank"><img src="http://img.youtube.com/vi/6jKi34irylo/0.jpg"
alt="LW-Modo Usage" width="240" height="180" border="10" /></a>

Pedro Alpiarça dos Santos has provided a Youtube Video showing the use between Houdini, Blender and Lightwave.

<a href="http://www.youtube.com/watch?feature=player_embedded&v=PFFQxb3nMvw
" target="_blank"><img src="http://img.youtube.com/vi/PFFQxb3nMvw/0.jpg"
alt="LW-Modo Usage" width="240" height="180" border="10" /></a>

# TODO:

* Houdini:  figure out how to get Morphs/Blendshapes integrated
* Maya:     figure out how to get Morphs/Blendshapes integrated
* Cinema4d: Implementation
* 3DsMax:   Implementation
* XSI:	    Implementation
* Sketchup: Implementation
* Unreal:   R&D to see if its possible to implement
* Unity:    R&D to see if its possible to implement
