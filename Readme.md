# Keymap for 34 key keyboard
![alt text](resources/keyboard-layout-all-layers.png)

To edit the keyboard, edit the ./config/cradio.keymap

With each push to the repository a new firmware is built via the .github workflow. 
Then attach one halve to the computer via usb. Set it into usb mode by [double click on the reset button](https://zmk.dev/docs/user-setup#flashing-uf2-files). Copy the right firmeware to each halve. It does not have to be renamed. When the file is copied, the usb-drive automatically disconnects and the firmware is enabled.

## General Thoughts

Use key combos for common keys: Escape, Enter, Backspace,[CapsWord](https://zmk.dev/docs/behaviors/caps-word), Tab

## Home Row Mods
Use [home-row-mods](https://precondition.github.io/home-row-mods#gacs)

![alt text](resources/keyboard-layout-HomeRowMods.png)

## Layer Change Keys
* Hold RH0 for Numbers Layer 
* Hold LH0 for Navigation Layer
* Hold LH1 for Symbols layer
* Hold c or , for Umlaut Layer
* Hold RH1 for function Layer
* Hold h for Braces Layer
* Hold 

On all layers except from 0, the free thumb keys do not trigger a layer change, they do the same thing as on the base layer, but with enabled repeat. That way these layer change keys can be repeated.

## Combos
* j+k Backspace
* d+f Escape
* f+j Capsword
* k+l Enter
* s+d Tab

![alt text](resources/keyboard-layout-Combos.png)

## Base Layer
ortholinear qwerty

LH1 tab, LH0 enter, RH0 space, RH1 backspace 
![alt text](resources/keyboard-layout-Base.png)

Here all other layers start.

## Umlaut Layer (hold v or m)
each umlaut on it's laut.
Euro, Dollar and @ are on the umlaut layer.
![alt text](resources/keyboard-layout-Umlaute.png)

## Navigation layer (hold LH0)
Navigation as in vim


If possible iso keyboard keys or combos are mapped to their vi counterpart, so that the same keys can be pressed in vi normal mode and in keyboard navigation mode.

![alt text](resources/keyboard-layout-Nav.png)

## Numbers and Symbols (hold RH0)
All numbers and some (math) symbols are on this layer. 

![alt text](resources/keyboard-layout-Num.png)

## Symbols (hold LH1)
Home row for fast access to vi keys.
Also top row keys were inspired by https://getreuer.info/posts/keyboards/symbol-layer/index.html


## Braces and Brackets (hold h)
Closing braces are mostly written by the editor, so we only have to type the opening part. These are placed on the home row keys.
Also most comment keys are on the brace layer.

![alt text](resources/keyboard-layout-Brace.png)

## Function Keys Layer (hold RH1)
Here are all function keys plus media keys plus bluetooth switches. The function keys follow the number keys.

![alt text](resources/keyboard-layout-Function.png)

## Key Naming
All keys in this document are named by the default qwerty character on the key. 
The thumb keys are named after this schema from [zmk-nodefree-config](https://github.com/urob/zmk-nodefree-config). This library is also used for defining the keymaps.
```
╭─────────────────────┬─────────────────────╮
│ LT4 LT3 LT2 LT1 LT0 │ RT0 RT1 RT2 RT3 RT4 │
│ LM4 LM3 LM2 LM1 LM0 │ RM0 RM1 RM2 RM3 RM4 │
│ LB4 LB3 LB2 LB1 LB0 │ RB0 RB1 RB2 RB3 RB4 │
╰──────────╮  LH1 LH0 │ RH0 RH1  ╭──────────╯
           ╰──────────┴──────────╯
```
## TODO
* home row mods with more delay, so that they do not trigger during rapid typing / role
* put shift onto RH1, remove the backspace and FUN layer functionality there
* trigger the FUN layer via the combination of the two right thumb keys RH0 and RH1
* put backspace on Nav layer RH0, del on Nav layer RH1
* asterisk on symbols layer LT2 and pipe and ampersand onto symbols layer, use LT1, LT2 and LT3.
* make the backspace and del key repeat
* put colon from right thumb to RM4 on symbol layer
* use ctrl+c, ctrl+x and ctrl+v for cut copy paste in nav mode on LM2, LB2 and LB0

