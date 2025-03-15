# EasyPrintedStages
A set of 3D printed open sourced motion stages for scientific and laboratory work compatible with the gridfinity standard. The latest "stable" (version printed and tested) release can be found on the printables linked below. Please consider going there and linking/downloading as it helps me out!
There are two different compatible stages in this ecosystem, a linear and rotary stage. A Z stage, pitch stage, and motorised stages are currently under development. You may see those in this repo but they are "alpha" versions uploaded to the master branch for collaborators to test before we fully release them. 

This readme is long but includes all the instructions you need to build and assemble the stages. ==IF PRINTING A LINEAR STAGE CHECK THE LEADSCREW PRINTING GUIDE FIRST FOR BEST RESULTS==.
##Content:
- Build Options for All Stages
- Linear Stage Specific Build Options
- Linear Stage Printing Instructions
- Linear Stage Assembly Instructions
- Rotary Stage Prtinting Instructions
- Rotary Stage Assembly Instructions


# Build Options for All Stages:
The design is built to be as modular as possible and users are encouraged to download FreeCAD and export the model to 3mf files for printer directly from the CAD files instead of using those provided. Numerous mounting solutions are also provided for the stage. 
## Optional Gridfinity Standard Mounting Plate:
The FreeCAD design makes use of the Gridfinity Workbench within FreeCAD. Users can find instructions on how to install and use this workbench under its associated page Gridfinity Workbench. A 2x2 unit Gridfinity base plate is provided in the design that can be screwed into the base of the stage. Additionally a 4x4 unit bolt together mesh is provided to act as a starting point for mounting a Gridfinity based stage system. 
![Pasted image 20250202160743](https://github.com/user-attachments/assets/ff7d15ff-24de-43c8-a503-f85c00ee6068)
Mounting bolts for the Gridfinity base plate go through the magnet holes on the plate base. __Note: If you make a custom base larger than 2x2u, you will need to quickly pocket the holes all the way through the plate. This has already been done on the provided 2x2u base.__
![Easy Stage In Mesh Cover 1](https://github.com/user-attachments/assets/df74fe93-2d87-4c07-8c64-df5cae036cf0)
## Optional Top Plate
![Pasted image 20250202161026](https://github.com/user-attachments/assets/827090ae-8969-43a3-beb9-6630fcedf227)
An optional top plate can be printed with the design. It mounts via 4 M3 bolts in the corners of the plate. The other 2 holes in the plate are for locking bolts, these holes go all the way through the top plate of the stage and allow a longer 25mm M3 bolt to be tightened down into the base of the stage, locking it in place. This can be used to lock the stage in a desired position. 

The mounting plate features a grid of 2.6mm diameter holes, these are the perfect size for M3 bolts to thread into without the need for threaded inserts. The holes are spaced 5mm apart to make designing custom mounting hardware as easy as possible. Some hardware for this plate has been provided, namely the Easy Stage Clamp. 
### How to make a custom mounting plate:
Open the design in FreeCAD and activate the Mounting Plate Body. The final operation is the one that pockets all the mounting holes, simply deleting this operation or copying the body from the previous operation will yield a blank plate that can be modified however is 
![Pasted image 20250202161508](https://github.com/user-attachments/assets/725fd63e-87e5-4191-9d9a-8c41669cf904)
![Pasted image 20250202161528](https://github.com/user-attachments/assets/05c06205-0a7a-4408-bb8b-61339d77a7e3)
## How to Mount Other Stages From The Ecosystem:
All of the Easy Printed Stages can be mounted to each other via the holes on their top.
![Cover Linear Best](https://github.com/user-attachments/assets/2d9b9e12-ff10-45a9-acaf-8bae10577890)
==NOTE ON ROTARY STAGE== Only two mounting bolts are accessible, these should be more than enough to hold it down but because of how the case halves are tightened down together a second pair of holes would never line up. 
# Linear Stage Specific Build Options:
##Rubber Band For Anti-Backlash
You can loop a rubber band between the threaded nut and the two holes where the adjustor protrudes from the base to apply a constant force onto the lead screw. This is generally not needed if printed at higher tolerance but was included for users using older printers without input shaping. 






