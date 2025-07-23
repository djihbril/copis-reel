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
>    * ### Frame and bed assembly
>      ![Frame & bed assembly](frame_&_bed.jpg)
>    * ### Completed 3D printer with test print
>      ![Completed 3D printer with test print](assemby_&_test.jpg)
>    * ### Belt tensioner print
>      ![Belt tensioner](belt_tensioner_print.jpg)
>    * ### Pan and tilt large gear printing
>      ![Pan & tilt large gear printing](pan&tilt_large_gear.jpg)
> *  A full-size `COPIS` machine consists of 2 chambers - usually stack on top of each other - each with 3 gantries offering X/Y/Z/Pan/Tilt movements in order to position a cradle-mounted camera for high-resolution picture taking. The `Python` client allows an operator to define a 3D path with desired nodes at which to take pictures and handles distribution of the nodes to each camera based on range; with optional collision detection . We opted for the Canon EOS camera line (80D and later RP) because it offered programmatic operation via the `Canon EDSDK`, with an available `Python` module. The client interfaces with each gantry via a custom controller board with a `C99 (ISO/IEC 9899:1999)` firmware, over I²C (Inter-Integrated Circuit) serial bus. It interacted directly with each camera via USB using the `Canon EDSDK` API. My team and I built and delivered one such machine (among others) to the `Harvard Museum of Comparative Zoolozy (MCZ)`:
>    * ### Harvard MCZ COPIS build day 1
>      ![MCZ build day 1](mcz_day_1.JPG)
>    * ### Harvard MCZ COPIS build day 2
>      ![MCZ build day 2](mcz_day_2.JPG)
>    * ### COPIS full frame
>      ![full frame](full_frame.jpg)
>    * ### COPIS full assembly with lighting and diffuser sheets
>      ![Full assembly](full_assembly.jpg)
>    * ### COPIS installed gantries and cameras close-up
>      ![Installed gantries](installed_gantries.jpg)
>    * ### COPIS gantries
>      ![Gantry assemblies](gantry_assemblies.jpg)
>    * ### COPIS Z/Pan/Tilt axes assemblies
>      ![Z/Pan/Tilt assembly](z_pan_tilt_assembly.jpg)
>    * ### COPIS workshop with motors, instruments and tools
>      ![Workshop](workshop.jpg)
>    * ### COPIS assembly station
>      ![Assembly station](assembly_station.jpg)
>    * ### COPIS controllers rail
>      ![controllers rail](controllers_rail.jpg)
>    * ### COPIS controller (hardware version 3) close-up
>      ![Controller](controller.jpg)
>    * ### COPIS hall-effect limit sensors for calibration and homing
>      ![Limit sensors](limit_sensors.jpg)
> *  Each `COPIS` chamber was designed to be versatile enough to accommodate artifacts from a 2ft x 2ft archeological object (single chamber on a surface setup) to a 1 mm mounted insect specimen with label data with reasonably high throughput, yet affordable enough to fit within grant budgetary constraints. To that effect, a full setup excluding the cameras has been meticulously design to fit within a $10k to $20k budget, as opposed to comparable industrial solutions that can get upwards of $200k. 
Upon taking photos of an artifact 3D reconstruction work is typically done by feeding the image to a `3D Photogrammetry` software like `RealityScan (formerly RealityCapture)` or `Meshlab`. [Our 3D models](https://sketchfab.com/yalepeabodymuseum) are hosted on the `Sketchfab` platform:
>    * ### Mask reconstruction in Meshlab
>      ![Mask modeling: Meshlab](Mashlab_mask.jpg)
>    * ### Reconstruction in RealityCapture (before texturing): [Bird-shaped Pottery Bank from the Yale Peabody Museum Anthropology Collection](https://sketchfab.com/3d-models/ypm-ant231383-a45e8e277b8040359a79e4e282b4ec69)
>      <video controls src="RC_pottery.mp4" title="Pottery modeling: RealityCapture"></video>
>    * ### Imaging session: pinned insect
>      ![Pinned insect](pinned_insect.jpg)
>    * ### Imaging session: pinned chrysalis
>      ![Pinned chrysalis](pinned_chrysalis.jpg)
>    * ### Imaging session: [Spindle whorl from the Yale Peabody Museum Anthropology Collection](https://sketchfab.com/3d-models/ypm-ant131826-c26b0a4ce0564970b709c90840ad97d7)
>      ![Spindle whorl](Spindle_whorl.jpg)