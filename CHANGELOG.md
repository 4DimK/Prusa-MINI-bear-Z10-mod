# Change Log

## [v0.1] - 07/03/2023 
Initial upload.

## [v0.11] - 08/03/2023 
- Fixed slight misalignment of X axis belt by raising the idler side belt lock system by 0.52mm. 

## [v0.12] - 09/03/2023
- Fixed Y axis belt holder alignment. 
- Added display holder and remaining electronics. 
- Added end caps in assembly, as they were provided by gregsaun.
- Organized STEP assembly, assigned proper names to all components.

## [v0.13] - 10/03/2023
- STEP file clean up and orient with Z upwards.
- Changed Y-motor-mount to the one shared by gregsaun ([link](https://github.com/gregsaun/prusa_i3_bear_upgrade)) as it seems more robust and provides better contact with the motor surface.
- Fixed internal gaps within parts, at least the ones I accidentally found.

## [v0.14] - 11/03/2023
- Updated Z-top-brackets to fix rod center misalignment introduced after  Z-motor-mount alignment fix.
- Added bolt head slot in Z-motor-brackets. 
- Cleaned up source CAD files and uploaded pre-printing state .f3z and .step files.

## [v0.2] - 12/03/2023
- Modified the MK3S Bear Y-motor-mount as to allow maximum Y travel for the Mini. 
- Fixed Z axis profiles y-axis offset at the position to allow full cover of print-bed. 
- Further stitching of internal gaps of MB-x-idler-right.

## [v0.21] - 18/03/2023
- Added build-helpers (remixed from gregsaun's Prusa Bear). One to set the Y-rod distance and the other for the Z-profile distance. 

## [v0.22] - 21/03/2023
My Mini+ Z threaded rod length was measured to be 309mm, which is different from the ones present in the CAD I started with (it safe to say now that the entire CAD has been modified). This affects the Z 2040 profile as well as the 10mm linear rod length. 
- Z profiles are now adjusted to a more reasonable length of 349mm and the linear rod properly adjusted as well.

## [v0.23] - 23/03/2023
- Added T-slot groove for MB-z-top-bracket and MB-z-motor-bracket since I accidentally used T-slot profiles for my Z axis. This feature is grouped in Fusion360 files and suppresses to leave V-slot groove for default.
- In MB-z-motor-bracket added a fillet in the motor entry slot, as to ease side insertion with a slight push. This is because there is no room to insert the motor from underneath after the bracket is fixed in place.

## [v0.24] - 24/03/2023
The T-nuts I had in stock appeared to have a difficulty tightening and fixing the component to the profile. 
- Added an additional cut in the v-slot groove (of all relevant parts) as to provide some extra turns.

## [v0.25] - 25/03/2023
- Added gregsauns Bear Z motor leadscrew caps and cable clips. Updated sources files.

## [v0.3] - 27/03/2023
Realized that MK3S and Prusa MINI use different leadscrew specifications, hence gregsauns leadscrew caps are not compatible with this mod. 
- Designed and tested new MINI(+) compatible leadscrew caps for TR8x4(p2x2) as per link. I used 0.2mm tolerance, which works well with my MINI. 

If you need different tolerance just adjust the `OffsetFaces` feature in Fusion. 