My preferred key bindings for both Linux and Windows.

Make use of caps lock, remap arrow keys to { i, j, k, l } and extra stuff.

For [Linux](#linux) and for [Windows](#windows)

# Linux
## input-remapper 
https://github.com/sezanzeb/input-remapper
### /home/user/.config/input-remapper/config.json
```json
{
    "version": "1.4.1",
    "autoload": {
        "AT Translated Set 2 keyboard": "capsl. + jkli = arrows",
        "Logitech USB Keyboard": "capslock + jkli = arrows",
        "Ducky Ducky One2 Mini RGB": "CAPSL. + jkli = arrows",
        "Corsair Corsair K70R Gaming Keyboard": "CAPSL + jkli = arrows",
        "Keyboard K850 Keyboard": "capsl + jkli = arrows",
        "Dell KB216 Wired Keyboard": "caps + asdf = arrows",
        "winkeyless.kr ps2avrGB": "capsl. + jkli = arrows",
        "Microsoft Microsoft Ergonomic Keyboard": "CAPSL. + jkli = arrows"
    },
    "macros": {
        "keystroke_sleep_ms": 10
    },
    "gamepad": {
        "joystick": {
            "non_linearity": 4,
            "pointer_speed": 80,
            "left_purpose": "none",
            "right_purpose": "none",
            "x_scroll_speed": 2,
            "y_scroll_speed": 0.5
        }
    }
}
```
### /home/user/.config/input-remapper/presets/name_of_keyboard/'capsl. + jkli = arrows.json'
```json
{
    "mapping": {
        "1,58,1": [
            "disable",
            "keyboard"
        ],
        "1,58,1+1,36,1": [
            "Left",
            "keyboard"
        ],
        "1,58,1+1,37,1": [
            "Down",
            "keyboard"
        ],
        "1,58,1+1,38,1": [
            "Right",
            "keyboard"
        ],
        "1,58,1+1,23,1": [
            "Up",
            "keyboard"
        ],
        "1,58,1+1,30,1": [
            "disable",
            "keyboard"
        ],
        "1,58,1+1,30,1+1,23,1": [
            "mouse(up, 5)",
            "mouse"
        ],
        "1,58,1+1,30,1+1,38,1": [
            "mouse(right, 5)",
            "mouse"
        ],
        "1,58,1+1,30,1+1,37,1": [
            "mouse(down, 5)",
            "mouse"
        ],
        "1,58,1+1,30,1+1,36,1": [
            "mouse(left, 5)",
            "mouse"
        ],
        "1,58,1+1,30,1+1,57,1": [
            "BTN_LEFT",
            "mouse"
        ],
        "1,58,1+1,30,1+1,40,1": [
            "wheel(10, down)",
            "mouse"
        ],
        "1,58,1+1,30,1+1,26,1": [
            "wheel(10, up)",
            "mouse"
        ]
    }
}
```
## AutoKey
[AutoKey](https://github.com/autokey/autokey) needs to be installed for Linux. This can be downloaded within Ubuntu package manager. The scripts can be found [here](linux/autokey).

At first caps lock has to be changed to function as the **hyper** key. This can be done with **Gnome Tweak Tool**.

| Shortcut                         | Output                           |
| -------------------------------- | -------------------------------- |
| CAPSLOCK + { i, j, k, l }        | { Up, Left, Down, Right }        |
| CAPSLOCK + CTRL + { i, j, k, l } | ALT + { Up, Left, Down, Right }  |
| CAPSLOCK + ALT + { i, j, k, l }  | CTRL + { Up, Left, Down, Right } |
| CAPSLOCK + { u, o }              | { Home, End }                    |
| ALT + { i, k }                   | { PageUp, PageDown }             |

Move the scripts to the directory `~/.config/autokey/data/`.

## Terminator
Terminator is used as a terminal and scripts can be found [here](linux/terminator).

| Shortcut                                | Output                                                         |
| --------------------------------------- | -------------------------------------------------------------- |
| CAPSLOCK + CTRL + Alt { k, l }          | Create new tab to the { bottom, right }                        |
| CAPSLOCK + CTRL { i, j, k, l }          | Focus the tab to the { top, left, bottom, right }              |
| CAPSLOCK + ALT + SHIFT + { i, j, k, l } | Increase/Decrease tab size to the { top, left, bottom, right } |
| CTRL + Shift + w                        | Close  tab                                                     |
| CTRL + Shift + c                        | Copy text                                                      |
| CTRL + Shift + v                        | Paste text                                                     |
| ALT + { i, k }                          | { PageUp, PageDown }                                           |

Move the script to the directory `~/.config/terminator/`.

## Tilda
Tilda is used as a dropdown terminal and the scripts can be found [here](linux/tilda).

This adds the terminal to the op of the screen by pressing `CapsLock + T`.

Move the script to the directory `~/.config/tilda/`.

# Windows

## AutoHotKey
[AutoHotKey](https://autohotkey.com) needs to be installed for Windows. The scripts can be found [here](windows/autohotkey).

| Shortcut                         | Output                           |
| -------------------------------- | -------------------------------- |
| CAPSLOCK + { i, j, k, l }        | { Up, Left, Down, Right }        |
| CAPSLOCK + ALT + { i, j, k, l }  | CTRL + { Up, Left, Down, Right } |
| CAPSLOCK + CTRL + { i, j, k, l } | ALT + { Up, Left, Down, Right }  |
| CAPSLOCK + { u, o }              | { Home, End }                    |
| ALT + { i, k }                   | { PageUp, PageDown }             |
| CAPSLOCK + { y, h }              | { PageUp, PageDown }             |

### Automatically start up
 1. Find the script file, select it, and press Control-C.
 2. Start **Run** and write `shell:startup`.
 3. Right click and choose **Paste Shortcut**. The shortcut to the script should now be in the Startup folder.

 If you need to run it as administrator either make sure the scripts is set up to administrator or start Command Prompt as administrator and run the scripts within.

 ## CMDer

| Shortcut                                | Output                                                         |
| --------------------------------------- | -------------------------------------------------------------- |
| CAPSLOCK + CTRL + Alt { k, l }          | Create new tab to the { bottom, right }                        |
| CAPSLOCK + CTRL { i, j, k, l }          | Focus the tab to the { top, left, bottom, right }              |
| CTRL + Shift + w                        | Close  tab                                                     |
| CTRL + Shift + c                        | Copy text                                                      |
| CTRL + Shift + v                        | Paste text                                                     |
| ALT + { i, k }                          | { PageUp, PageDown }                                           |

Download font [FiraCode](https://github.com/tonsky/FiraCode) and [FlottFlott](https://www.dafont.com/flottflott.font)

# macOS

## Karabiner-Elements
[Karabiner-Elements](https://pqrs.org/osx/karabiner/index.html) needs to be installed for macOS. The `karabiner.json` file with the profile can be found [here](macOS/Karabiner).

| Shortcut                                                  | Output                                                    |
| --------------------------------------------------------- | --------------------------------------------------------- |
| CAPSLOCK + { i, j, k, l }                                 | { Up, Left, Down, Right }                                 |
| CAPSLOCK + ⌘ COMMAND + { i, j, k, l, Backspace, Delete }  | ⌥ OPTION + { Up, Left, Down, Right, Backspace, Delete }   |
| CAPSLOCK + ⌥ OPTION  + { i, j, k, l, Backspace, Delete }  | ⌘ COMMAND + { Up, Left, Down, Right, Backspace, Delete }  |
| CAPSLOCK + { u, o }                                       | { Home, End } (*)                                         |
| SHIFT + Backspace                                         | Delete                                                    |

* Home and End aren't very useful on macOS. Similar functionality can be achieved with OPTION + Up (start of line), and OPTION + Down (end of line).
Note that those would be COMMAND + Up and COMMAND + Down with the provided bindings.

### Adding to Karabiner
> :warning: **If you already use Karabiner**: follow the advanced steps to avoid loss of current settings.

Copy [karabiner.json](macOS/Karabiner/karabiner.json) to your Karabiner config directory.
This will result in Karabiner reading two profiles; 'Default macOS' and 'CAPSLOCK + IJKL'.
Select 'CAPSLOCK + IJKL' and you are all set!

#### Advanced: copying only the modifications
If you already have your own profile and you only want to add the complex modifications, follow these steps.

In [karabiner.json](macOS/Karabiner/karabiner.json) locate the profile 'CAPSLOCK + IJKL' and copy all the desired modifications from the 'rules' section (lines 153 to 844).

# Git
Helper tools for git

## Git alias
[gitalias.txt](git/gitalias.txt) contain git aliases to be added to your git config.
