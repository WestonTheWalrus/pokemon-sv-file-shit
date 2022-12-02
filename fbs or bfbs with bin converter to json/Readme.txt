 " " " " " " " " " " " " " " " " " " " " " " " " " " " " "	
 " ______ _       _   _            __  __                "
 " |  ___| |     | | | |          / _|/ _|               "
 " | |_  | | __ _| |_| |__  _   _| |_| |_ ___ _ __ ___   "
 " |  _| | |/ _\`| __| '_ \| | | |  _|  _/ _ \ '__/ __|  "
 " | |   | | (_| | |_| |_) | |_| | | | ||  __/ |  \__ \  "
 " \_|   |_|\__,_|\__|_.__/ \__,_|_| |_| \___|_|  |___/  "
 " ______ _____ _   _                                    "
 " | ___ \_   _| \ | |                                   "
 " | |_/ / | | |  \| |                                   "
 " | ___ \ | | | . \ |                                   "
 " | |_/ /_| |_| |\  |                                   "
 " \____/ \___/\_| \_/                                   "
 "  _____                           _                    "
 " /  __ \                         | |                   "
 " | /  \/ ___  _ ____   _____ _ __| |_ ___ _ __         "
 " | |    / _ \| '_ \ \ / / _ \ '__| __/ _ \ '__|        "
 " | \__/\ (_) | | | \ V /  __/ |  | ||  __/ |           "
 "  \____/\___/|_| |_|\_/ \___|_|   \__\___|_|           "
 "                                                       "
 " By duckdoom5 & Inidar                                 "
 "                                                       "
 "                                                       "
 " For support, find us on Discord:                      "
 " https://discord.gg/bCkhsSdwSY                         "
 "                                                       "
 " " " " " " " " " " " " " " " " " " " " " " " " " " " " "  

Tool Description

Want to make changes to the game's config BIN files? This tool is for you.

Flatbuffers BIN Converter Tool can be used to deserialize flatbuffers, allowing you to freely edit the BIN files Scarlet and Violet use as config files.

It can be used with both .fbs and .bfbs schema files, and will convert files from .bin --> JSON and back again.

Warning: There is always a risk when working with bat files. Please follow all instructions carefully, do not modify the scripts unless you know what you are doing, and never download this tool from anywhere but this post.

Scripts created by Duckdoom5 and Inidar

----------------------------------------------------
Need more help ?
Join Inidar Academy on Discord:
https://discord.gg/bCkhsSdwSY

------------------------------------------------------------------------------------------

Usage Instructions

TLDR: First, extract the tool zip into a working folder and add flatc.exe to the folder root. 
Second, put the .bin or JSON you want to convert and it's corresponding fbs/bfbs schema into the Input folder. 
Finally, run the appropriate .bat file to complete the conversion.

Want more details? Read on!

----------------------------------------------------

1. Preparing the Converters
Make a new folder and extract Flatbuffer_BIN_Converter.zip inside it. All files and folders extracted from Flatbuffer_BIN_Converter.zip must be contained in this new folder.


*****Warning*****  
Do not use these scripts anywhere except your working folder. 
That means don't run them loose on your desktop, in a downloads folder, or alongside any other important files.
They will never delete any files and would most likely do nothing at all, but they *are* designed to modify certain files in the same directory as themselves. 
So to be safe, stick to best practice and use a working folder when running the scripts.
*****Warning***** 


----------------------------------------------------

2. Acquiring flatc.exe
Visit this link (https://github.com/google/flatbuffers/releases) and download the latest Windows.flatc.binary.zip.

Unzip it, then drag flatc.exe into the root of the folder you created in step 1 (beside the Converter .bat files)

----------------------------------------------------

3. Finding Config Files
If you already know what you want to modify, you can skip to step 4. If you need ideas, read on.

To find interesting files to mod, download pkNX, open your SV romfs, then use the 'Master Dump' option. In particular, be sure to extract the romfs/world/data folder to find many config files. 

If you don't know how to use pkNX, please see my Pokemon Legends tutorials on Gamebanana.

This will give you a huge amount of files to go through and get ideas, but do not use the .bins or JSONS from pkNX to make mods. Extract and convert everything yourself with Trinity instead to avoid issues.

Alternatively, you can find and extract game files yourself by completing up to Step 4 in this tutorial: (https://gamebanana.com/tuts/15506) 


----------------------------------------------------

4. Running the Converters
You will need 2 files to complete the conversion: a .bin file and a .bfbs.

The .bin file will contain the game config, and .bfbs is a schema that can be used to deserialize it. 
These 2 files will be stored together in the same folder of the romfs, so if there is no .bfbs file beside the .bin you want to modify, you need to make your own schema (which is well beyond the scope of this tutorial). 
Note: .fbs files are also accepted.


To begin the conversion:

Put the .bin file and it's corresponding .bfbs or .fbs file in the Input folder.

Your folder directory should now look like this:
Input-->something.bin, something.bfbs
Output
Convert_To_BIN.bat
Convert_To_JSON.bat
flatc.exe

Finally, run Convert_To_JSON.bat.

Your JSON file will then appear in the Output folder.

To convert from JSON to .bin, it's the same process: put your JSON file in the Input folder, the correct .bfbs file in the folder root, then run Convert_To_BIN.bat.

Remember: Each .bin file will have it's own .bfbs schema, so make sure you have the correct .bfbs file in the folder root. Using the wrong schema may give an error, or it may output a non-functional BIN.

----------------------------------------------------

5. Final Notes
This tutorial barely scratches the surface of flatbuffers.

If you are willing and able to improve the scripts or add more, send me a message and I'll make an update.

------------------------------------------------------------------------------------------

Feedback & Acknowledgments
Huge thank you to Duckdoom5 for taking my terrible tiny scripts and making them 1000x more useful and user-friendly, and thanks again mv_oripoke and CraftyBoss for all your help with learning about this.

To see more of Duckdoom5's work, check out his github:
https://github.com/JelleInfinity


Also thank you so much Jamorhi, itskurtly, VulgrPixel, Omegatron3423, TheSnorlaxBoi, H3roDude, and Ænigma for your support -- Legends, all of you.

All my mods are always free, but if you want to support my work and get your own shoutout, check out my Patreon or buy me a coffee below:)
https://www.patreon.com/Inidar
https://ko-fi.com/inidar


