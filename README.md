# COPIS Reel
> A page that showcases my `Mechatronics` skills via my work with the [Computer Operated Photogrammetric Imaging System (COPIS)](http://copis3d.org/) at the Yale Peabody Museum - Biodiversity &amp; Data Sciences Lab.
The repo with my contributions to the `COPIS` `Python` desktop client application is [here](https://github.com/YPM-Informatics/COPISClient/commits/main/?author=djihbril).

## Hardware
> The `COPIS` hardware was entirely conceptualized, designed and implemented in house. 
> *  Part of my job was to help test it out, develop a user manual and iterate over the current version with judicious improvements such as suggesting the use of a slip ring at the Z/Pan axes boundary to replace wires that frequently twisted, tangled and frayed over time:
>    * ### Slip-ring assembly
>      ![Slip-ring assembly](slipring_assembly.jpg)
>    * ### Installed slip-ring - close-up
>      ![Installed slip-ring - close-up](installed_slipring.jpg)

> * All plastic parts were designed and 3D printed onsite. To that effect we used a `Original Prusa i3 MK3` 3D printer kit which I assembled:
>    * ### Extruder assembly
>      ![Extruder assembly](extruder.jpg)
>    * ### Frame assembly
>      ![Frame assembly](frame.jpg)
>    * ### Frame & bed assembly
>      ![Frame & bed assembly](frame_&_bed.jpg)
>    * ### Completed 3D printer with test print
>      ![Completed 3D printer with test print](assemby_&_test.jpg)
>    * ### Belt tensioner
>      ![Belt tensioner](belt_tensioner_print.jpg)
>    * ### Pan & tilt large gear printing
>      ![Pan & tilt large gear printing](pan&tilt_large_gear.jpg)
> *  A full-size `COPIS` machine consists of 2 chambers - usually stack on top of each other - each with 3 gantries offering X/Y/Z/Pan/Tilt movements in order to position a cradle-mounted camera for high-resolution picture taking. The `Python` client allows an operator to define a 3D path with desired nodes at which to take pictures and handles distribution of the nodes to each camera based on range; with optional collision detection.