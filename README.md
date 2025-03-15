# EasyPrintedStages
A set of 3D printed open sourced motion stages for scientific and laboratory work compatible with the gridfinity standard. The latest "stable" (version printed and tested) release can be found on the printables linked below. Please consider going there and like/download as it helps me out!
There are two different compatible stages in this ecosystem, a linear and rotary stage. A Z stage, pitch stage, and motorised stages are currently under development. You may see those in this repo but they are "alpha" versions uploaded to the master branch for collaborators to test before we fully release them. 

This readme is long but includes all the instructions you need to build and assemble the stages. __IF PRINTING A LINEAR STAGE CHECK THE LEADSCREW PRINTING GUIDE FIRST FOR BEST RESULTS__.
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
__NOTE ON ROTARY STAGE__ Only two mounting bolts are accessible, these should be more than enough to hold it down but because of how the case halves are tightened down together a second pair of holes would never line up. 
# Linear Stage Specific Build Options:
##Rubber Band For Anti-Backlash
You can loop a rubber band between the threaded nut and the two holes where the adjustor protrudes from the base to apply a constant force onto the lead screw. This is generally not needed if printed at higher tolerance but was included for users using older printers without input shaping. 

# Linear Stage Printing Instructions:
The design should be printed in 2 separate sets. These are documented here. __PLEASE CHECK THE LEAD SCREW SETTINGS BELOW OR IT WILL FAIL TO PRINT!__
## Bulk, Low Tolerance Components
Parts in this set are: 
- Base Plate with Integrated Gridfinity
- Shim
- Upper
- Adjuster Cap
- Base
- M3 5mm Spaced Mounting Plate
- 2u Gridfinity Base Plate

__Recommended Materials for This Set:__
- PETG --> Best overall and chemically resistant so good for use in the lab. 
- PETG CF --> Much stronger than regular PETG but surface is rougher and parts can be less clean/may need sanding. Also more expensive.
- PLA --> Cheapest and easiest to print but not chemically resistant so use only in non-wet lab's. 

You can also use pretty much anything else you want provided its mechanically hard but increasing the strength of these parts does little for the designs overall strength since the weakest point is the printed lead screw. 

__Print Settings and Other Info:__
- You can get away with a 0.6 or 0.8mm nozzle on this set to improve print time but the fit/finish will be worse. __0.4mm is recommended__. There is no need to use high detail slicer parameters. 
- __Enable support__ for the Base and Base Plate with Integrated Gridfinity parts, the overhand here needs it. Tree supports are recommended and if a __threshold angle of 30 degrees__ is used in the slicer only this region of the design will be supported by Tree's. //this was tested in Bambu, Orca, and Prusa slicer. 

3mf project files for this set have been made for Bambu Studio (specifically for the A1 Mini but can easily be adapted to their other printers) and Prusa slicer, they can be found within the GitHub for the project. 
## High Tolerance Threaded Parts
Parts in this set are: 
- Adjuster
- Thread Block Modelled

__Recommended Materials for This Set:__
- PETG --> Best if you only have a low temperature printer.
- ASA --> Best if you have a high temperature printer but chemical resistance isn't a concern. 
- PET --> Best for high temperature and chemical resistance but hard to print well. 

*Note on PLA: You can use it but it may not be strong enough nor is it chemically resistant.* 

*Note on CF/GF reinforced filaments: They can be used here but there is a concern about their abrasive nature wearing down the threads over time.* 

__Print Settings and Other Info:__
- Use a 0.4 or 0.2mm nozzle.
- Use 100% infill.
- Use the highest detail setting on the slicer of your choice, less because of detail, more because it will slow the printer down making the long tall lead screw print easier. 
- If you cannot use the provided 3mf for the Adjuster __HAVE A LOOK AT IT FIRST BELOW__. Custom painted on supports are used to stabilise the tall and wobbly part and make it print well. Open that model and see how I've done it before trying to print it yourself. I used the paint on custom support tool in the slicer with the tree supports. Make sure not to paint them onto the threads or it will ruin the threads, paint them on just after the threads finish at the top of the adjuster. 
![Supported Leadscrew](https://github.com/user-attachments/assets/4d872afb-a097-4150-9092-01bd1e9da707)
![Support Enforcers on Outside of Leadscrew](https://github.com/user-attachments/assets/ef297552-49c6-4022-b1e4-29d0ab04c4dd)
![Support Enforcer in Top of Leadscrew](https://github.com/user-attachments/assets/fe59586f-f406-4d3a-8bb6-f79fbc783a86)

# Linear Stage Assembly Instructions:
## Important Note: 
Use silicone grease on the way and lead screw to make the stage move easier and last longer. 
## Step 1: Thread the Adjuster
Apply a small amount of Silicone Grease to the adjuster tip and to the holes made for it in the base of the stage, thread the adjuster through the block and then apply the end cap with an M3x5mm bolt. At this stage you should also apply Silicone Grease to the ways of the stage. You're assembly should look like the one seen below:
![Step 1 Photo](https://github.com/user-attachments/assets/03c9d5e7-084c-4484-9933-a3caa1697b98)
__Note: The direction of the little triangle on the top of the thread block doesn't matter, its for a different project that re-uses these parts.__
## Step 2: Mount Upper
Insert the longer M3 bolts into the side of the upper but leave some space, you only want about 2mm of the bolt to protrude into the way, as seen below: 
![step 2 alt angle photo](https://github.com/user-attachments/assets/400ed7e0-e7fc-419f-82ef-5670183a11f5)
Slide the upper over the lower assembly from __STEP 1__, you dont need to put the shim in yet. You'll feel the top seat itself down onto the threaded block with a click, once you feel this you can tighten the two M3 bolts on the top.
![step 2 no way](https://github.com/user-attachments/assets/458d5830-bb69-4c87-81ac-8324d8009bc8)
__Note: There is a vernier gauge modelled on the side of the base and the top piece, make sure you have the top piece the right way round if you plan on using these. The top is ambidextrous so if you get this wrong the stage will still work.__ 
You can now slide the shim in, make sure the holes on the side of the shim face the bolts you partially inserted earlier.
![step 2 way insert photo](https://github.com/user-attachments/assets/b7ac2b79-8e08-478d-8cfe-bbdbb79a37f3)
Slide the shim all the way in and then start to tighten the bolts on the side. 

__Important:__ Tighten each bolt a little at a time alternating between them. After each bolt check to see if moving the stage is hard, if its hard to move you've tightened the bolts too much and should back them off about half a turn. These bolts are what constrain the stage, you want no play (wobble) in the top of the stage but still want to be able to move the stage with little/no resistance. 
![step 2 way flush](https://github.com/user-attachments/assets/25500639-99ac-4be1-a843-c41567527427)
## Step 3: Mount Any Addons
You can now mount the top plate of a Gridfinity base. In the images above the Gridfinity base was already installed. You're finished stage should look something like this:
![Easy Stage Linear Cover Photo](https://github.com/user-attachments/assets/5f4bd505-85dc-451e-a86b-60f7bc51b798)
__Note: The stage shown in the image has been etched with a fibre LASER to engrave the text and decals seen__ 

# Rotary Stage Printing Instructions
## Cycloid 
Print the cycloid in PETG (or any other hard material thats not fiber reinforced). Use a 0.4mm or 0.2mm nozzle and high quality print settings. __NO SUPPORT IS NEEDED__
## Worm Gear
Generally the automatic organic supports of most modern slicers can print the work gear just fine with no needed additions. Print with a 0.4 or 0.2mm nozzle (ideally 0.2mm to make the action smoother). See the image below for how it was supported during testing. Printing at 100% infill is recommended for durability but not strictly necessary.
![Pasted image 20250216155126](https://github.com/user-attachments/assets/61eaec93-4b9c-4f08-be58-602e12f719c8)
## All Other Parts
These can be printed in any material with either a 0.4 or 0.6mm nozzle. For the parts seen in the Easy Rotary Stage Assembly Instructions below, PETG-CF filament was used with a 0.6mm nozzle. 

# Rotary Stage Assembly Instructions:
## Important Note: 
Just as with the Linear Stage: Silicone Grease is your friend, use more than you think and wipe the excess off after! This stage can bind when first assembled due to small printing defects, spin the stage via the platform not the adjuster a few time to wear those defects down and smooth the action of the stage. 

## Step 1: Mount the Cycloid Gear
Mount the cycloid gear as seen below. The triangle embedded onto the base of the triangle and on the base of the stage will aid in alignment.

__DO NOT FULLY TIGHTEN THE BOLTS.__

Leave about 3mm space between the gear and the base plate. You tighten these later once the rest of the stage is installed. 
![Gear Only On Top](https://github.com/user-attachments/assets/17d0016e-42d5-4d01-be52-52619a283ff1)
![Side Cinematic View](https://github.com/user-attachments/assets/14630576-581d-4390-9668-083aa9adb412)

## Step 2: Slide the Front Under the Gear
You can now tighten the bolts on top so that there is no play between the cycloid gear and the front of the stage.
![Cycloid Gear Installed](https://github.com/user-attachments/assets/caa66422-5ae4-4192-a02a-a38cd69271a6)

## Step 3: Insert the Worm Gear Into the Back Piece with the Spacer Shim
Slide the worm gear into the back of the case. See the pictures below. Its had to see the spacer, its the small "puck" looking part with a small indent on one side, this indent faces away from the worm gear and is pressed against by an M3 bolt which compresses the worm gear to prevent play in the mechanism. 
![Shaft Installed Dark](https://github.com/user-attachments/assets/080e0054-fbcb-4243-992b-a24276a86514)
__ENSURE THE SPACER PUCK IS BETWEEN THE WORM GEAR AND THE CASE__
The depression in the centre of the puck should face the case not the worm gear. An M3 bolt screws through the side of the case and pushed against this, removing the play in the cycloid gear. 
![Adjustor Shim View](https://github.com/user-attachments/assets/4944e9d0-eb58-4e4a-ae22-7fdd43acb2d4)
Its hard to see in the image below but an M3 bolt screws into that hole to compress the worm gear and remove any play in the mechanism. 
![SIde Adjustor BOlt](https://github.com/user-attachments/assets/a2a772aa-de5f-478c-a78f-6894263e04b9)
## Step 4: Bolt the Front and Back of the Case Together
![Assembled Mechanism Top View](https://github.com/user-attachments/assets/8c959ccc-2fc3-4d7b-b0a6-f45cc699b83f)
There are two M3 counter bored holes on the worm gear side of the casing. Into these two M3 bolts can be placed that will mate with the other side of the case. Tighten these until the two halved are together and can move freely with no play. You may need to adjust this over time as the gears wear into each other. Avoid over tightening. This design will always have backlash due to the lower tolerances on the cycloid gears that make it possible. 

__You will need a long Hex Bit to reach the M3 bolts__
![Lower Fully Assembled](https://github.com/user-attachments/assets/00fe87f9-f1b0-4120-85a1-bdb854c9edf7)

## Step 5: Mount the Aligner Plate
The plate with two channels on it fits into the grooves on the front and base parts of the case, there are two bolt holes that lock this into the case and then prevent any movement. These are M3 bolts and have counter bored holes. The other holes in this piece are for either the Gridfinity Standard mounting plates, to mount the box to other Easy Printed Stages, or to mount a universal mounting plate. 
![Top Bolted On Best](https://github.com/user-attachments/assets/1e12d812-728b-456d-8077-e4c220c1560b)

## Step 6: (OPTIONAL) Mount to Other Stages, Gridfinity Base, Mounting Plate etc..
![Cover Gridfinity 4](https://github.com/user-attachments/assets/c5a9c9fd-dba3-405c-b750-d1fcb593e884)











