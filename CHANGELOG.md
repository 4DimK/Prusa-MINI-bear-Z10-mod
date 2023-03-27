[07/03/2023] - Edit 0: Initial upload.

[08/03/2023] - Edit 1: Fixed slight misalignment of X axis belt by raising the idler side belt lock system by 0.52mm. Updated STEP file to v0.1 and the relevant pictures.

[09/03/2023] - Edit 2: Fixed Y axis belt holder alignment. Added display holder and remaining electronics. Also added end caps in assembly, as they were provided by gregsaun. Organized STEP assembly, assigned proper names to all components, updated to v0.3 and relevant pictures. 

[10/03/2023] - Edit 3: STEP file clean up and orient with Z upwards. Updated to v0.4.

[10/03/2023] - Edit 4: Changed Y-motor-mount to the one shared by gregsaun ([link](https://github.com/gregsaun/prusa_i3_bear_upgrade)) as it seems more robust and provides better contact with the motor surface. Also fixed internal gaps within parts, at least the ones I accidentally found. Updated STEP to v0.5.

[11/03/2023] - Edit 5: Updated Z-top-brackets to fix rod center misalignment introduced after  Z-motor-mount alignment fix. Updated STEP to v0.6.

[11/03/2023] - Edit 6: Added bolt head slot in Z-motor-brackets. Cleaned up source CAD files and uploaded pre-printing state .f3z and .step files.

[12/03/2023] - Edit 7: Modified the MK3S Bear Y-motor-mount as to allow maximum Y travel for the Mini. Fixed Z axis profiles y-axis offset at the position to allow full cover of print-bed. Further stitching of internal gaps of MB-x-idler-right. Updated source files.

[18/03/2023] - Edit 8: Added build-helpers (remixed from gregsaun's Prusa Bear). One to set the Y-rod distance and the other for the Z-profile distance. Updated sources files.

[21/03/2023] - Edit 9: My Mini+ Z threaded rod length was measured to be 309mm, which is different from the ones present in the CAD I started with (it safe to say now that the entire CAD has been modified). This affects the Z 2040 profile as well as the 10mm linear rod length. Z profiles are now adjusted to a more reasonable length of 349mm and the linear rod properly adjusted as well. Updated sources files.

[23/03/2023] - Edit 10: 1) Added T-slot groove for MB-z-top-bracket and MB-z-motor-bracket since I accidentally used T-slot profiles for my Z axis. This feature is grouped in Fusion360 files and suppresses to leave V-slot groove for default. 2) In MB-z-motor-bracket added a fillet in the motor entry slot, as to ease side insertion with a slight push. This is because there is no room to insert the motor from underneath after the bracket is fixed in place. Updated sources files.

[24/03/2023] - Edit 11: The T-nuts I had in stock appeared to have a difficulty tightening and fixing the component to the profile. Added an additional cut in the v-slot groove (of all relevant parts) as to provide some extra turns. Updated sources files.

[25/03/2023] - Edit 12: Added gregsauns Bear Z motor leadscrew caps and cable clips. Updated sources files.

[27/03/2023] - Edit 13: Realized that MK3S and Prusa MINI use different leadscrew specifications, hence gregsauns leadscrew caps are not compatible with this mod. Designed and tested new MINI(+) compatible leadscrew caps for TR8x4(p2x2) as per link. I used 0.2mm tolerance, which works well with my MINI. If you need different tolerance just adjust the OffsetFaces feature in Fusion. Updated sources files.