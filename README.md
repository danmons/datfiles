# What?
DAT files are used for ROM management tools like [ClrMAMEPro](https://mamedev.emulab.it/clrmamepro/), [SabreTools](https://github.com/SabreTools/SabreTools), Romulus, [RomVault](http://www.romvault.com), [RomCenter](https://www.romcenter.com) and others.  They contain the files needed with correct names and checksums to allow you to rebuild a working set from other collections you may have.

# Why?
The FPGA [MiSTer project](https://github.com/MiSTer-devel/Main_MiSTer/wiki) provides the checksums (in MD5 format) of the final output ROM needed.  These are generated via scripts that concatenate several smaller ROMs from the [MAME project](https://www.mamedev.org) together.  Problem is if one of your files are missing or wrong, it's impossible to know which one is at fault.  DAT files can assist to verify and rename the source files correctly.

# How?
Look up guides on how to use [ClrMAMEPro](https://mamedev.emulab.it/clrmamepro/) (specifically the "Rebuild" function).  There are many well written ones.  I'll try to put links in here later.  Other ROM managers are mentioned above, but I haven't used them.  Anything that works with standard DAT files (standard across the entire preservation/emulation scene) should work. 

# Note
4 of the 95 ROMs in this set fail the final checksum when the MiSTer build_rom scripts are called.  They are:
* catacomb
* woodpeck
* mrtnt
* pengo

It appears as if all of these are bad dumps.  However, the checksums produced match those [documented by SmokeMonster](https://github.com/SmokeMonsterPacks/EverDrive-Packs-Lists-Database/blob/master/EverDrive%20Pack%20SMDBs/MiSTer.txt), so either the build_rom scripts are wrong, or Smokemonster and I are wrong. :)
