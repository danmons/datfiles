# What?
DAT files are used for ROM management tools like [ClrMAMEPro](https://mamedev.emulab.it/clrmamepro/), [SabreTools](https://github.com/SabreTools/SabreTools), Romulus, [RomVault](http://www.romvault.com), [RomCenter](https://www.romcenter.com) and others.  They contain the files needed with correct names and checksums to allow you to rebuild a working arcade set from other collections (e.g.: [MAME](https://www.mamedev.org/)) you may have.  This isn't for console ROM management.  If you want that, check out [SmokeMonster's Everdrive Packs](https://github.com/SmokeMonsterPacks/EverDrive-Packs-Lists-Database) instead.

# Why?
The FPGA [MiSTer project](https://github.com/MiSTer-devel/Main_MiSTer/wiki) provides the checksums (in MD5 format) of the final output arcade ROM needed.  These are generated via scripts that concatenate several smaller ROMs from the [MAME project](https://www.mamedev.org) together.  Problem is if one of your files are missing or wrong, it's impossible to know which one is at fault.  DAT files can assist to verify and rename the source files correctly.

# How?
Look up guides on how to use [ClrMAMEPro](https://mamedev.emulab.it/clrmamepro/) (specifically the "Rebuild" function).  There are many well written ones.  I'll try to put links in here later.  Other ROM managers are mentioned above, but I haven't used them.  Anything that works with standard DAT files (standard across the entire preservation/emulation scene) should work. 

# Bugs
There are 106 files this DAT file covers currently.  There are 3 that do not build correctly according to MiSTer build_rom.sh and build_rom.bat expected final checksums.  They are:
* catacomb.zip
* ckongpt2.zip
* uniwars.zip
