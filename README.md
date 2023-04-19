# Method for making Icons
This is my method for Creating .Ico files and for creating DLL that store .Ico files. 

## Required software
    1. Inkscape 1.1.2 
    2. Gimp 2.10.35
    3. Microsoft Visual Studio, Version 17.2.5, 
      a) Desktop development with C++
## Optional software
    1. Resource Hacker, Version 5.1.7 
# Design the Icon in Inkscape
    1. Open Inkscape 
    2. New From Template → Icon… → Select Icon size: → Select a Standard size: 16, 32, 48, 64, 96, 128, or 256.
    3. Create from Template
    OR
    1. Open Inkscape
    2. File → Document Properties…
    3. Document Properties panel → Custom size:
        1. Set Units: px
        2. Set both Height and Width to same Standard sizes: 16, 32, 48, 64, 96, 128, or 256.
    4. Design Icon paths
    5. Group paths
    6. Center Design to the center of page border 
    7. Save
# Import SVG into Gimp create Icon File
    1. Open Gimp
    2. File → New
    3. Set Image size Width and Height to size of the SVG importing, recommend 256 px.
    4. Layer → Transparency → Add Alpha Channel
    5. Remove background by pressing the Delete key
    6. Drag and drop the designed SVG on the layer.
    7. Make sure the SVG size matches the size set in Step 3.
    8. Click Ok.
    9. Delete Layer Background
    10. File→ Export…
    11. Update the file name to end with the .ico extension 
    12. Export
# To create a Ico DLL project in Visual Studio
    • Visual Studio needs to install Desktop development with C++. 
    1. Open Visual Studio → Create a New Project dialog box.
    2. At the top of the dialog, set Language to C++, set Platform to Windows, and set Project type to Library.
    3. From the filtered list of project types, select Dynamic-link Library (DLL), and then choose Next. 
      (If DLL is not shown then Desktop development with C++ needs to be installed.)
    4. Input file Name → Create.
    5. Solution Explorer → right click on Resource files → Add →  New Item…
    6. Visual C++ → Resource → Select Resource file (.rc)
    7. Click Add button
    8. Double click Resource.rc
    9. Resource View → right click on Resource.rc→Add Resource…
    10. Add Resource → Import…
    11. Select File Type to Icon files (*.ico)
    12. Select .ico File(s) → Open
    13. Save Project
    14. Select dllmain.cpp window
    15. Build DLL.
    16. Navigate to file location in the Output window.
    17. Copy the DLL to desired storage location.
