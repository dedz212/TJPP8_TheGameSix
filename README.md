# TheGameSix
TheGameSix is The Jackbox Party Pack 8 mod that adds a sixth game to the list<br>
Created for modifiers so as not to replace the existing original game.

## STEPS
### **1.** Unpack the archive<br>
  First you need to unpack the archive, you'll see there `"games"` folder, this folder you replace in `"...\Steam\steamapps\common\The Jackbox Party Pack 8"`. Done, start the game and you will see the sixth game in the list.

### **2.** Replace with a mod<br>
  To run a sixth game, in `"TheGameSix"` folder (which is in the `"games"`) must be all files from one of the five games from Party Pack 8. If you for example want to add a modified game to the list of sixth games, for example: tWoET, then you must first copy all of the original files (in the example: tWoEP) and paste into `"TheGameSix"` folder, only then replace the files there with a mod.

### **3.** The ability to run<br>
  Okay, you did it, except why is it still listed as `"The Game Six"` and the description `"Game 6, pretty crazy, right?"`?

#### **3.1** content.json<br>
  Well, don't worry, you should find the `PartyPack` folder, open it, and go into the `content.json` file, any way you like. Then, scroll down until you will not see `"name": "TheGameSix"`, then what you need to do is to specify the main swf, which the game will be defined and run, in the example with tWoEP is `TheWheel.swf`, next, these are tags, in our case in this file we find the `"name": "TheWheel"`, and copy data from there with the tags and paste into yours. After that, we have tagline and menu, leaving it as it is, then we have video and audio. Same as from `"name": "TheWheel"` we copy and paste there. And that's it, this step is done!

#### **3.2** Localization.json<br>
  In this file we find `"MENU_GAME_NAME_6"` and `"INFO_TAGLINE_GAME_6"` and replace a information them with whatever you need.

### **4.** The image on the menu.
  You have 517x429 png instead of a cake? This can be fixed, there you can insert your cake or just copy it from an already created cake from Jackbox Games. Just go to `PickerContent.swf` (in `PartyPack` folder) and then the most important thing...

#### **4.1** Same size
  If the image is the same size as 517x429 go to the section `"image"` and find `"DefineBitsLossless2 (481)"`, press Right-click the mouse and `"Replace..."`, then you find the image you want to replace. I say it again, the image you want to replace should be 517x429.
At last save and run the game. If everything looks quite nice and pleasing to the eye, you can not do step 4.3.

#### **4.2** Size other
  If the image is smaller or larger, go to the section `shape` and find `DefineShape (477)`, then you Right-click the mouse and `Replace - Update Bounds...`, then you find the image you want to replace. Okay, you did this, but because the size is different, the image can find the left, right, top, bottom, more and/or less. Because of this is extra work, but you can handle it too.
To start, save and run the game. If everything looks nice and pleasing to the eye, you don't have to do the next step.

#### **4.3** mhh, not pretty..
  You go to `frames` and `"frame 96"`. Then go to `"PlaceObject 81"`, a separate tab should appear in the guide, there you find the `"Edit"` button, open the `"matrix"` section there, and change the value in `"translateX"` and/or `"translateY"`. If for some reason the right hand box does not appear, then click on `"PlaceObject 81"` and `"Raw edit"`, click on `"Edit"`, open the "matrix" section there, and change the value in `"translateX"` and/or `"translateY"`.
Note that this is if you want to move them to the right, left, up, and right. If you change `translateX` to a higher value, it moves to the right. If `translateY` to a higher value, it moves down! When you change, remember how many numbers are different from the original, you need this!
  If you want just increase or decrease scale, then this is responsible `"scaleX"` and `"scaleY"`, increase or decrease the same, proportional changes also need to remember how many numbers different from the original.
> P.S. You can use `"Free Transform"` but it does not always work correctly. Be vigilant!<br>

Then when you moved the image as you want, open `PlaceObject 80` and change as before, for example: if you moved the X to +500 in `PlaceObject 81`, then in `PlaceObject 80` move X to +500.

### **5.** Launch Party Pack<br>
  Save and see how it looks in the end. If everything looks pleasing to the eye, congratulations, you've added your TheGameSix to what you wanted. If nothing works, re-read the text, you may have done something wrong. (For example: you didn't put the game in from Party Pack 8.)<br>
  If you have any questions, go to [Discord Server](https://www.discord.gg/FsfSdVKcwq)


==================================================================<br>
- tWoET - [the Wheel of Enormous Trolling](https://www.jackboxmods.ga/main#h.kfwpkj6296vd)<br>
- tWoEP - [the Wheel of Enormous Proportions](https://jackboxgames.fandom.com/wiki/The_Wheel_of_Enormous_Proportions)
