# Blockdata / Entitydata Editor:
*Designed for 1.12.2, should work with older versions.*

This macro helps you edit blockdata or entitydata, by showing you a list of all the data the block/entity contains. 

**Set Up:**
- Place `$${@&oldchat = %CHAT%}$$` in the onChat Event
- Use a file include eg `$$<blockdata.txt>`

**Usage:**
- Look at either a tile entity block*(Anything with blockdata)*, or an entity.
- Activate the script using a button or a keybind. 
- If you looked at an entity, you will need to select the target manually, such as `@e[type=pig]`.
- It will show you a gui menu with all of the block/entities data. 
- You can then click and change the value. When you are done, press enter. 
- The value you just changed will be saved, and you can continue editing the values.
- If you see a (0) or (1) at the beginning of the list, that number is the index of the item. If you specifically want to change a item of a index, keep this index number the same. 
- To append new items to the list, you can just type the data directly into the input box. 
- If you want to stop the macro, double click `cancel` and the script will stop.
- Finally, press escape to close the menu, and the blockdata will be changed. 

**Others:**
- A limitation is when changing the block data of really complicated things (such as colored signs and command blocks) might cause the list to not be grouped properly. 
- This macro tries it's best to reduce the output command size, but if it goes over 256 characters, you will need to put it in a command block. 
- You can also use my targetselector.txt macro to choose the entities for the entity data. 
- If you are wondering why there are ［］，characters, they are used to prevent the prompt array action from make 2 items when it is supposed to be 1 item. 
- If there are any bugs/questions, please tell me! 

**Link:**
https://github.com/KeeMeng/Macro-Keybind-Mod-Scripts/blob/master/blockdata.txt
