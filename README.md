# X68K_Pico_PSU_v2
SHARP X68000 PicoPSU Power Adapter v2

This project builds on the original X68K_EZ_Pico_PSU by moving the AC-DC converter inside the original X68000 PSU case, making for a very clean, OEM look.

Instructions:

(1) Manufacture and assembled the board using the parts from the BOM.

(2) The AC-DC converter requires minimal standoffs from the PCB. These standoffs should be conductive so that the PCB ground meets the converter ground.

(3) While you can use a 2-prong AC power cable, I've used a 3-prong (grounded) AC power cable in the application as suggested by @leonkiriliuk. Strip the outer shielding and expose the hot (white), neutral (black), and ground (green) wires. Cut a section of the hot and neutral and connect those from the original power switch to the AC-DC converter. If you have a 3D printer, print the enclosed X68K_AC_Cable_Strain_Relief.stl file and slip it over the power cable; this is a strain relief that will "plug the hole" of the PSU case. Attach the AC cable hot and neutral to the other leads on the original power switch. Attached the ground wire to the AC-DC converter's ground post.

(4) Plug in your PicoPSU and attached the +12VDC and ground to the corresponding terminals on the AC-DC converter.

(5) When connecting your original X68000 harness to the PCB, @leonkiriliuk has suggested that the PicoPSU's ATX molex may not provide enough amperage for the floppy disk drives (FDD). It is advisable to wire the FDD leads from the X68000 harness to the 4-pin molex attached to the PicoPSU or your FDD may not work. v3 of this board will fix this by routing the 4-pin molex to a dedicated terminal on the PCB.

Notes on this build:

(1) The AC-DC converter used is a low wattage unit. There are higher wattage units available in the series that fit just fine. I went with the 75W unit because of cost.

(2) It's important to match the power output of your AC-DC converter with the power rating of the PicoPSU. 

(3) While you do not need a 3-prong AC power cable, it is advisable to use one as it will ground the entire electrical system of your X68000 to Earth ground.
