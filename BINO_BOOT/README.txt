copy the "bino_boot" folder loader to Arduino "harware" folder

Burn bootloader thru your arduino the available board is the MightyCore Standar 644/324 at 16/20 Mhz clock only

copy the spicific bino loader "RUVICSAB.BIN" to your SD card according to your board and clock select from the "bino_loader" folder 324/644 - 16/20

to compile your own project just used the MightyCore Board......

	Click "Sketch" and Click "Export compiled binary" 
		OR 
	Hit "" Ctrl + Alt + S ""

To locate the "HEX" files 
	Click "Sketch" and Click "Show Sketch Folder"
		OR
	Hit "" Ctrl + K ""

To convert Hex to Bin

Use the "HEX" files without bootloader......
avr-objcopy -I ihex -O binary "YOUR PROJECT".hex "NEW PROJECT NAME".BIN
"NEW PROJECT NAME" must be at most 9 CHARACTER ONLY!!!!!!!!

SD Card Format is FAT32....
Copy the files to your SD Card....
