# RecursiveExport
Simple plugin for Sketch.app to recursively export exportable layers in a selected naming scheme.
I was surprised it didn't exist so I wrote it. If anyone knows an easier way to do this let me know.

## What it does 
When selecting a layer in your canvas and running the script, the script
will prompt for an export directory and a desired export structure.
Then it traverses your layers and exports each layer that has been
marked exportable in all of the export formats defined for that layer [^1].

## Install

- Download the plugin from the **Releases** tab in this repo. 
- Unzip and doubleclick on the `.sketchplugin` file to install. 
- It should now appear in Sketch.app under the menu item `Plugins`.

## Screenshots

So given

<img width="229" alt="Screenshot 2024-12-14 at 11 14 45" src="https://github.com/user-attachments/assets/54c83fe2-aed5-40c3-881d-484d563c5aee" />

It asks

<img width="338" alt="Screenshot 2024-12-14 at 11 01 22" src="https://github.com/user-attachments/assets/98180df5-1991-458e-92c4-e651700a8008" />

And exports either 

<img width="431" alt="Screenshot 2024-12-14 at 11 15 15" src="https://github.com/user-attachments/assets/ed6ad854-3344-4e8e-9b0e-1aa0085f8cf4" />

or 

<img width="278" alt="Screenshot 2024-12-14 at 11 16 45" src="https://github.com/user-attachments/assets/fc10b2af-b52e-4d8a-bbb3-9bc0fef7c5ff" />

or just a plain list of files named the same as the layer. 

But you can do the latter without the plugin, just in Sketch > File > Export



[^1]: It does apply the prefixes and postfixes defined in the export format, but it ignores the size settings. If anyone can get that working, let me know.
