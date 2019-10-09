# What?
DAT files are used for ROM management tools like ClrMAMEPro, Romulus, RomVault, RomCenter and others.  They contain the files needed with correct names and checksums to allow you to rebuild a working set from other collections you may have.

# Why?
The MiSTer project provides the checksums (in MD5 format) of the final output ROM needed.  These are generated via scripts that concatenate several smaller ROMs from the MAME project together.  Problem is if one of your files are missing or wrong, it's impossible to know which one is at fault.  DAT files can assist to verify and rename the source files correctly.

# How?
Look up guides on how to use ClrMAMEPro.  There are many well written ones.  I'll try to put links in here later.

# Note
4 of the ROMs in this set fail the final checksum when the MiSTer build_rom scripts are called.  They are:
* catacomb
* woodpeck
* mrtnt
* pengo

It appears as if all of these are bad dumps.  However, the checksums produced match those documented by SmokeMonster, so either the build_rom scripts are wrong, or Smokemonster and I are wrong. :)
