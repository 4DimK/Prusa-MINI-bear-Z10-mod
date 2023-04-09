# Change Log

## [v1.0] - 08/03/2023
### Changed
- MK3S-extruder-body: Added bolt head cavity in the probe holder. 
- Spool-holder: Increased side diameter to easier insert M4 bolt.

### Fixed
- MB-FS-lever: adjusted gap for more reliable operation
- Increased overall robostuness of remixed electronics case

## [v0.9] - 08/03/2023
### Added
- Filament sensor functionality. The following parts are modified.
    - MB-extruder-motor-plate: Extra travel space is accommodated for the FS-lever inverted function.
    - MB-FS-lever: The lever is modified to provide the inverted (not mirrored) function of MK3S which complies with the MINI firmware sensor interpretation.
    - **Important** MK3S-extruder-body: The filament sensor cable provided for the MINI has inverted plug polarity when oriented to be used with the MK3S. The plug red and black wires need to be swapped. The part is edited to move mirror the plug alignment groove.
- MB-spool-holder is now extended with a filament guide, inspired from the images of the new MK4 holder. 


### Fixed
- X axis max travel was 3mm short (177mm). This is fixed by updating the 2040 top and front-rear profiles, to 220mm and 300mm respectively. This affects the following parts:
    - X-idler-right and left: X-axis rod cavities are shortened by 2mm each.
    - MB-helper-Y: Length increased by 2mm.
    - X axis belt lenght: 4mm of extra length is required.
- Z-top-bracket: The tolerance is increased from 0.2mm to 0.25mm to allow easier rod insertion. Also, following from the aforementioned combination of the bracket with the end-cap, the extra thickness allows some room for Z rod length mismatches (in case the rods are cut manually).
- X-axis-endstop-spacer is not extended to sit on top of the right idler. This effectively constrains the spacer from rotating. The spacer also does not limit the tramming function.
    - The spacer provides 3.5mm of clearance. Just enough to not tram to the leadscrew. This can easily be incorporated within the idler itself. The reason to not do that is that in case another extruder design is used, the required clearance might be different, or not at all.

### Changed
- Top Z endcaps and Z-top-brackets are now a combined part. This results in a more robust bracket that can also be used to tram align the X axis.
- In MK3S-extruder-body, the probe has been brought 3mm close to the extruder. 
- MB-display-holder: added extra thickness around the M3 bolt as to allow insertion of a M3 locknut.
- MB-electronics case: This is now a complete remix of the original design from 3DPGVA. The reason is that there was not enough space to incorporate the extra length of the wires I had and the lead was not closing properly. I took the change to add extra cable covers, inspired both from MK3S as well as the MK4 electronics boxes.


## [v0.81] - 06/03/2023
### Added
- X-axis-endstop-spacer. The x axis idlers are to be updated as to avoid sensorless homing by side kicking the leadscrew. For versions prior to v0.81 it is recommended to use the spacer on the top X axis rod attached next to right idler as to avoid damaging the Z leadscrew.
- MB-spool-holder. This is a draft version and is not printed yet. Not even sure if I will be using a top place spool holder. Either way, this remixed out of PR supplied MK3S STL of their spool holder and modded to be attached on 2020 extrusion. There is also an insert with space for M4 bolt. That is meant to incorporate a filament guide.
- Added PRINT_PROFILES folder. Currently it includes a draft config bundle with only one Bear compatible profile (settings, filament and printer) derived from 0.2mm QUALITY @MINI for 0.4mm nozzle. All settings related to the extruder are copied from the equivalent MK3S profile. STL and SVG of ht the MINI heatbed are included if adding the visuals is of interest. These are directly downloaded from PrusaSlicer github [repo](https://github.com/prusa3d/PrusaSlicer/tree/master/resources/profiles/PrusaResearch).

## [v0.8] - 02/03/2023
### Added
- Pictures of the realized mod

### Changed
- Updated STL files for the following parts:
    - X-idler-left
    - X-idler-right

### Fixed
- X-idler-right and X-idler-right linear rod cavities for x-axis linear rods is shortened to meet the length of the stock rods for easy assembly.

## [v0.33] - 31/03/2023
### Fixed
- X-idler-right and X-idler-left bearing holes length is extended by 0.4mm as to make sure that the bearing sits below the top surface and not interfering with the POM nut. Also, a chamfer is added to it to ease the overhand printing.
- Y-belt-holder for the mini needs to allow room for the PCB heater center bolt head. A 6x3mm cavity is added in the center hole.
- CAD length of X-axis linear rods as taken from the original CAD I started with, is not in accordance with the stock rods. The length is fixed to 279mm. To make sure that both rods are symmetrically inserted between the idlers, 18mm bolts need to be fully inserted in the left idler.

## [v0.32] - 30/03/2023
### Fixed
- Y-motor-mount top surface was barely blocking the headbed rear bold head. Reduced thickness by 1mm to allow free move.
- Z-motor-mount hole for the 10mm rod had no tolerance applied. It is now set at 0.2mm.
- Z-top-bracket had a tolerance for 10mm rod set 0.085mm. That proved to small for my Mini. It is now also increased to 0.2mm.

## [v0.31] - 29/03/2023
### Changed
- Reduced and rounded Z rod length. Total axis travel possible is 206mm. Albeit, without changing the firmware max travel is set at 180mm from the bed surface.

## [v0.3] - 27/03/2023
### Changed
Realized that MK3S and Prusa MINI use different leadscrew specifications, hence gregsaun's leadscrew caps are not compatible with this mod. 
- Designed and tested new MINI(+) compatible leadscrew caps for TR8x4(p2x2) as per [Prusa MINI motor specifications](https://github.com/prusa3d/Original-Prusa-MINI/blob/master/DOCUMENTATION/ELECTRONICS/mini-motor-kit.pdf). Part tolerance is set to 0.2 mm, which should work well with any well working MINI(+). 

If you need different tolerance just adjust the `OffsetFaces` feature in Fusion. 

## [v0.25] - 25/03/2023
### Added
- gregsauns Bear Z motor leadscrew caps and cable clips. Updated sources files.

## [v0.24] - 24/03/2023
### Added
The T-nuts I had in stock appeared to have a difficulty tightening and fixing the component to the profile. 
- Added an additional cut in the v-slot groove (of all relevant parts) as to provide some extra turns.

## [v0.23] - 23/03/2023
### Added
- T-slot groove for MB-z-top-bracket and MB-z-motor-bracket since I accidentally used T-slot profiles for my Z axis. This feature is grouped in Fusion360 files and suppresses to leave V-slot groove for default.
### Fixed
- In MB-z-motor-bracket added a fillet in the motor entry slot, as to ease side insertion with a slight push. This is because there is no room to insert the motor from underneath after the bracket is fixed in place.

## [v0.22] - 21/03/2023
### Fixed
My Mini+ Z threaded rod length was measured to be 309mm, which is different from the ones present in the CAD I started with (it safe to say now that the entire CAD has been modified). This affects the Z 2040 profile as well as the 10mm linear rod length. 
- Z profiles are now adjusted to a more reasonable length of 349mm and the linear rod properly adjusted as well to 311mm.

## [v0.21] - 18/03/2023
### Added
- Build-helpers (remixed from gregsaun's Prusa Bear). One to set the Y-rod distance and the other for the Z-profile distance. 


## [v0.2] - 12/03/2023
### Fixed
- Modified the MK3S Bear Y-motor-mount as to allow maximum Y travel for the Mini. 
- Z axis profiles y-axis offset at the position to allow full cover of print-bed. 
- Further stitching of internal gaps of MB-x-idler-right.

## [v0.14] - 11/03/2023
### Added
- Bolt head slot in Z-motor-brackets. 
### Fixed
- Updated Z-top-brackets to fix rod center misalignment introduced after  Z-motor-mount alignment fix.
- Cleaned up source CAD files and uploaded pre-printing state .f3z and .step files.

## [v0.13] - 10/03/2023
### Changed
- STEP file clean up and orient with Z upwards.
- Changed Y-motor-mount to the one shared by gregsaun ([link](https://github.com/gregsaun/prusa_i3_bear_upgrade)) as it seems more robust and provides better contact with the motor surface.
### Fixed
- Fixed internal gaps within parts, at least the ones I accidentally found.

## [v0.12] - 09/03/2023
### Added
- Added display holder and remaining electronics. 
- Added end caps in assembly, as they were provided by gregsaun.
### Fixed
- Fixed Y axis belt holder alignment. 
- Organized STEP assembly, assigned proper names to all components.

## [v0.11] - 08/03/2023 
### Fixed
- Fixed slight misalignment of X axis belt by raising the idler side belt lock system by 0.52mm. 

## [v0.1] - 07/03/2023 
Initial upload.
