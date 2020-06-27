# Info for Jsoner.txt

## Functions:
Convert minecraft color codes/format codes into a json format, also supports click and hover events. (You can basically use this in game, instead of a online tool)

---

## Usage: 

### Chat Colors:
```
&0 Black         
&1 Dark Blue
&2 Dark Green    
&3 Dark Aqua
&4 Dark Red      
&5 Dark Purple
&6 Gold          
&7 Gray
&8 Dark Gray     
&9 Blue
&a Green         
&b Aqua
&c Red           
&d Purple
&e Yellow        
&f White
```
### Chat Format:
```
&l **Bold**
&o *Italics*
&m ~~Strikethrough~~
&n __Underline__
&k Obfuscated
&r Reset
```
### Special Format Function:
```
- Click Events:
  - Open URL: &U <URL> &U
    - Clicking the text opens a link
  - Run Command: &C <Command> &C
    - Clicking the text runs a command directly
  - Suggest Command: &S <Command> &S
    - Clicking the text types a command in chat, user needs to press enter manually
  - Insertion: &V <Text> &V
    - Shift clicking the text inserts something into the chat, user needs to press enter manually

- Hover Events:
  - Show Text: &T <Text> &T
    - Hovering over the text shows a tooltip (Tooltips can be colored using normal minecraft & codes too)
  - Show Item: &I <\"id\":\"*???*\",\"Count\":*???*> &I
    - Hovering over the text shows an item 
  - Show Entity: &E <Entity> &E
    - Hovering over the text shows an entity

- Others:
  - Scoreboard Value: &O <"score":{"name":"*???*","objective":"*???*"}> &O
    - Replaced with the score of a player
  - Selector: &P <@p/@a/@r/@s/@e/???> &P
    - Replaced with the selector name
  - Keybind: &K <Keybind> &K
    - Replaced with the key bind name
```
*Remember to have the special codes on both side, to enclose the input for that function.*

---

## Examples:
Shows `World` when hovering on "Hello":
```
&6&lHello&T&a&lWorld&T
```

Execute `/tp @p ~ ~20 ~` command when clicking "Teleport", shows `Up & Up` when hovering above "Up":
```
&6&lTeleport&C/tp @p ~ ~20 ~&C &e&lUp&TUp && Up&T
```

Shows a stone item when hovering above "Stone":
```
&7Stone&I\"id\":\"stone\",\"Count\":1&I
```

Shows a box with the text below:  
> Moo 

> Type: Cow
```
&lMilk&Etype:Cow,name:Moo&E
```

Shows "Hello USERNAME" with colors:
```
&c&lHello &e&l&P@p&P
```

Inserts ":)" to chat when shift clicking `Click to insert`:
```
&5&lClick to insert&V:)&V
```

Clicking on `spawn` runs the command "/spawn", and clicking `warp` gives you $$w list, and runs "/warp <value>" :
```
&9&lTeleport to &b&lspawn&C/spawn&C &a&lwarp&C/warp $$w&C
```

Shows the key bind for `key.jump`, usually it is "space": 
```
C&e&lJump is &a&l&Kkey.jump&K
```

---

## Others:
If you need any help, please contact my discord: TKM#6228

You can ask me for command help, and also how the script works, or anything else! Have fun!
