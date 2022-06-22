# Seawolf-Libraries
A collection of component libraries used in club PCB projects.

## Installing IntLibs
- Download repo as a zip or clone it to `C:\Users\Public\Documents\Altium\Projects`. DO NOT CLONE TO `AD19`, `AD20`, `AD21`, etc subdirectories! Just clone it to the projects folder.
- Double click each `IntLib` file you want to install. When prompted choose install **not** extract sources.
- The libraries will then be listed in the `Components` panel
- Libraries can be updated the same way. Either pull the repository (if cloned) or download a newer zip and double click and install each `IntLib` file to update.

## Adding Parts to URC_Lib
- Clone this repository to `C:\Users\Public\Documents\Altium\Projects`. Note that `Documents` may be shown as `Public Documents` in file explorer
- DO NOT CLONE TO `AD19`, `AD20`, `AD21`, etc subdirectories! Just clone it to the projects folder
- Double click the `URC_Lib.IntLib` file to open it. When prompted by altium choose `Extract Sources` this will create a folder called `URC_Lib`. This folder will contain the extracted `URC_Lib.SchLib` and `URC_Lib.PcbLib` files.
- To add a new part (not copy from a downloaded library)
  - Create a symbol in the `URC_Lib.SchLib` file. Give it the name of the part.
  - Create a footprint in the `URC_Lib.PcbLib` file. Give it the name of the part (or in some cases the name of the package type could be more appropriate).
  - Add a footprint to the symbol in the `URC_Lib.SchLib`. Browse in the `URC_Lib.PcbLib`
- To add a part from a downloaded library follow the same steps as above, but instead of creating new symbols / footprints copy / paste from the downloaded library's `SchLib` and `PcbLib` files. When the symbol is copied it will reference the footprint in the wrong `PcbLib` file so after copying both symbol and footprint go back and remove the footprint from the symbol, then add the correct one from `URC_Lib.PcbLib`.
