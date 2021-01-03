# Swap-Characters-Between-Seasons-Part-2
This tutorial will teach you to change the facial animations of characters.

# Beginning
First, you'll need the materials if you want to make S3 work in S4 for example or S4 in S1. It's limited for now but hopefully in the future there will be more options.
[Here are the materials you need to download.](https://www.mediafire.com/file/3f8o608trd84b06/Materials.rar/file)

You'll also need [ttarch](http://aluigi.altervista.org/papers/ttarchext.zip) to extract the files from ttarch files.
If you have the files then you are good to go for model swapping.

**CURRENT PROBLEMS:** Season 3 sadly doesn't work with any other season together, but it can work with any season by itself. Like if you plan to have Javier in S1, you'll have to have S3 characters otherwise everything will look invisible.

## STEP 1: Locate the ttarch files you need.
**Where can I find them?** It's real simple, just go to game's folder and you'll see a folder named Archives there. 

**Which files are necessary for model swapping?** In this step we'll only need to get data.ttarch2 and anichore.ttarch2

## STEP 2: Extracting the files.

**DATA:**

You'll need to create a notepad and paste this, of course you have to edit it because I don't know where the game is in your computer. Don't forget to create a folder named data as well, copy it's location then paste it to inside of "C:\data". Don't delete the " though.

```
ttarchext.exe -k 96CA999F8DDA9A87D7CDD9BB93D1BEC0D79171DC9ED98DD0D18CD8C3A0B0C695C39C93BBCCCCA7D3B9D9D9D08E93BEDAAED18D77D5D3A3 0 "C:\(the game folder)\Archives\data.ttarch2" "C:\data"
```

Examples: WDC_pc_WalkingDead204_data.ttarch2, WDC_pc_WalkingDead305_data.ttarch2, WDC_pc_WalkingDead404_data.ttarch2


**ANICHORE:**

You'll do the same method as you did for Data. Just rename the data.ttarch2 to anichore.ttarch2

```
ttarchext.exe -k 96CA999F8DDA9A87D7CDD9BB93D1BEC0D79171DC9ED98DD0D18CD8C3A0B0C695C39C93BBCCCCA7D3B9D9D9D08E93BEDAAED18D77D5D3A3 0 "C:\(the game folder)\Archives\anichore.ttarch2" "C:\data"
```

Examples: WDC_pc_WalkingDead204_anichore.ttarch2, WDC_pc_WalkingDead305_anichore.ttarch2, WDC_pc_WalkingDead404_anichore.ttarch2

After copying, pasting and editing is done then save the notepad files as .bat and put it near the ttarchext folder. Don't copy and paste all the codes together, seperate them! Because the program might not recognize what you are trying to do. Then open the .bat file and the rest will be done by the program.

## STEP 3: Renaming the necessary files.

**DATA:**

You'll have to rename all the ptable files with other character you want to swap with. 

For example, sk54_alvinFearB to sk61_javierFearB

Do this step until you rename all the files with the character you wanted to swap.

**ANICHORE:**

After exporting the files, rename the files like you did with the ptable files. Here's the files you need to rename:

**DIFFERENCES:**

S1-S2: (character)_eyes_down (for eye animation)
sk54_idle_(character)AngryC (for face animation)
(character)_face_blink (to make characters blink)

S3-S4: (character)_headEyeGesture_LookDown (for eye animation)
(character)_face_moodAngryC (for face animation)
(character)_face_eyesClosed (to make characters blink)

**OPTIONAL:**

S1-S2: (character)_face_browsGestureDown_add (for eyebrow animations)

S3-S4: (character)_face_browsDown_add (for eyebrow animations)

The difference is needed since you want to swap s2 character with s3 or whatever you are up to! But if you want to swap the characters who are in the same season, you don't need to check the difference.

## STEP 4: Testing
After you are done with renaming the files, put them into Archives folder. Also! Don't forget to use the materials, just in case if you forgot about it in the previous tutorial. 
Then open the game, to be sure go to character viewer and click on the lines to see if their mouth animations are working or you can check the animations as well, if they work well then congrats!
