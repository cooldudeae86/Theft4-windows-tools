Are you getting that pesky "NO STATIC BC TEXTURES FOUND :(" message when trying to run theft4? Are you running the game and find that you are driving the invisible boat mobile? Are you running an iphone 15 and below that doesn't support the bc textures like iphone 15 pro and later do? 

These are the theft4_inspect and theft4_stage tools (from https://github.com/KoreanSeats1/Theft4) that I rewrote from Mac OS M-series ARM64 architecture to work on Windows 11 x86-64 architecture with chatgpt.com. This is for people who have no mac to build and run these tools. You could create a hackintosh like I did to do it but that's besides the point. 

I made a youtube video guide here or you can follow written instructions below: https://youtu.be/EL5PgeHOetM

Note that you must provide your own game and update files, none are included with these tools. 
--------------------------------------------------------------------------------------------------------------------------------
<br>
===================================================================================
Now first you have to download the file in the releases section. ⪼------➢ 

I recommend first running theft4_inspect to make sure you have the correct version of the iso and update packages. To do this, open up a command prompt (cmd) and change the directory to the game-tools folder. 

    Go into windows-tools ⮞ build ⮞ then right click on the folder ⮞ game-tools ⮞ and click copy as path 
    
    In your command prompt, type in "cd" then a space then paste the path that you copied and hit enter 

    Now type in "theft4_inspect" space "path/to/game.iso" space "path/to/update.package" and hit enter 

    It should tell you first that the base game is supported and then after that the update is supported. 
    If it doesn't say that then you have the wrong versions of one or both of them. 
----------------------------------------------------------------------------------------------------------------------------------
<br>
===================================================================================
Now with your game file and update shown as supported, stay in the command prompt to run theft4_stage next. This will extract the needed files for theft4 to operate. 

    Type in "theft4_stage" space "path/to/game.iso" space "path/to/update.package" space "path/to/nameofnewfolder" 
    then hit enter (the nameofnewfolder should be a new folder that does not exist already) 

    Now it should run and you may have to wait a bit since it is extracting a lot of files. 
    I will say "staging verified" at the end when it is finished. 
-----------------------------------------------------------------------------------------------------------------------------------
<br>
===================================================================================
Once that is done, go to your "path/to/nameofnewfolder" location and copy the ⮞ game ⮞ folder inside of it to your iphone. Now on your iphone sideload the latest 0.3.2 theft4 ipa from the official github https://github.com/KoreanSeats1/Theft4 

Run theft4 on your iphone and once it says the game folder has been created, close the app. Then you will move the staged game files you copied from your computer earlier into the game folder that theft4 created inside of the files app. 

    It should look like this after you are finished: ⮞ Theft4 ⮞ game ⮞ common, xbox360, $SystemUpdate, aes_key.bin, 
    audio, audio.rpf, common.rpf, default.xex, default.xexp, update, xbox360.rpf

Now run theft4 on your iphone and if you need to prepare texture files, it will take 20-30 minutes for that to finish and then it should run the game! >o<

If you would like to say thanks for my hard work to fix these errors: Buy me a cup of green tea: https://throne.com/ae86skyline

Thank you to https://github.com/OZORDI/LibertyRecomp and to https://github.com/KoreanSeats1/Theft4 for making this game possible!
