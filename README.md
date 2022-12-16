# X68K_Pico_PSU_v2
SHARP X68000 PicoPSU Power Adapter v3

This project builds on the original X68K_EZ_Pico_PSU by moving the AC-DC converter inside the original X68000 PSU case, making for a very clean, OEM look.
For several years this board has revived a lot of dead X68000 Computers.

# Instructions:

	(1) Manufacture and assembled the board using the parts from the BOM.
	-Take the zipped gerber files to a PCB manufacturer such as JLCPCB and PCBWAY
	-Purchase parts in the BOM file by part number at an electronics parts distributor such as mouser, digikey, arrow etc.
	-Assemble!

	(2) While you can use a 2-prong AC power cable, I've used a 3-prong (grounded) AC power cable in the application as suggested by @leonkiriliuk. Strip the outer shielding and expose the hot (white), neutral (black), and ground (green) wires. Cut a section of the hot and neutral and connect those from the original power switch to the AC-DC converter. If you have a 3D printer, print the enclosed X68K_AC_Cable_Strain_Relief.stl file and slip it over the power cable; this is a strain relief that will "plug the hole" of the PSU case. Attach the AC cable hot and neutral to the other leads on the original power switch. Attached the ground wire to the AC-DC converter's ground post.

	(3) Plug in your PicoPSU and attached the +12VDC and ground to the corresponding terminals on the AC-DC converter.  This can be found on the datasheets. 
	Generally you will want to cut the barrel jack connector off of the Pico PSU and solder it to the output terminals from the AC/DC converter.

	(4) You will require spacers to hold the ACDC converter on the card.  The mounting holes are 3.5mm wide so any 3mm with washers or 3.5mm spacers will be fine.  Make sure they're quite short.

	(5) There is also an optional strain relief that can be 3D printed (STL). Helpful if you needed to add a new cable.

# Assembly recommendations:

	(1) Recommended AC/DC converters are the following models:
 
		VMS-100C-12
		EPP-120S-12
		RPS-120S-12
		VMS-120C-12
	
	They will fit with spacers on the mainboard per their respective datasheet. They output plenty of power for X68000.  
	
	(2) Recommended Pico PSU: The only recommended Pico PSU is the offical ones sold by mini-itx. 120 Watt plays very well with X68000. You can go higher if required.
		https://www.mini-itx.com/~picoPSU-120
		
		Generally the authentic ones will have a yellow connector and are purchased from mini-itx.  Sometimes these are sold from third parties.  However there are a lot of clones floating around.
		It is recommended to purchased a Pico PSU from mini-itx.  Clones are not recommended.
		
	(3) Wiring instructions
 
	All X68000 have a wiring harness attached to their power supply with multiple power cables.  This could be intimidating by people unfamiliar with their model.  
	Please check the Photos folder for clear indication to know where you need to connect the wires.
	
	For X68000 PRO:
	
	Some X68000 Pro in the wild have the 'Tetris PSU'  (this one) and some of the wiring instructions on the net might be confusing.  Please open your X68000 Pro PSU first to determine which type you have.
	The power supply designed below might be better for your needs:
	
	https://github.com/leaded-solder/x68000-pro-picopsu
		
		
		
		
