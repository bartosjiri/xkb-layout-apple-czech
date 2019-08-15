# Czech Apple keyboard layout
XKB layout for Czech Apple keyboard:

![Czech Apple keyboard layout](https://support.apple.com/library/content/dam/edam/applecare/images/cs_CZ/keyboards/czech_notebook.png "Czech Apple keyboard layout")


## Installation
1. Replace the default Czech layout with the modified one:
    ```
    sudo cp <path/to/file>cz /usr/share/X11/xkb/symbols/
    ```

2. Add the layout to option list:
	- Assuming you haven't done any previous modifications to your `evdev.xml` file, replace the layout options list:
      ```
      sudo cp <path/to/file>evdev.xml /usr/share/X11/xkb/rules/
      ```
	- Alternatively, add the following code to other Czech layouts in your `evdev.xml` file :
      ```
      <variant>
        <configItem>
          <name>apple</name>
          <description>Czech (Apple layout)</description>
        </configItem>
      </variant>
      ```
3. Activate the layout in your keyboard settings.

## Limitations
This keyboard layout does not affect modifier keys (Function, Control, Option/Alt, Command/Super). 
