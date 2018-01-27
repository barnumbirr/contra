

# contra
Everything I need for my [Contra 40% ortholinear keyboard](https://cartel.ltd/projects/contra).

## Parts

### Cartel Ltd.

* [Contra 40% ortholinear keyboard kit](https://mykeyboard.eu/catalogue/danck_397/)

### Aliexpress

* [Cherry MX Pink Plate Mounted Keyswitch](https://www.aliexpress.com/item/Wholesales-Cherry-Gateron-Silent-Zealio-Kailh-Box-Outemu-Ice-Purple-Switches-Shaft-for-Mechanical-Keyboard-GH60/32844881260.html)
* [2u PCB Mount Mechanical Keyboard Cap Stabilizer](https://www.aliexpress.com/item/OEM-Cherry-Style-PCB-mounted-PCB-Stabilizers-Satellite-Axis-7u-6-25u-2u-For-MX-Switches/32718144332.html)
* [XDA Blank Keycaps](https://www.aliexpress.com/item/XDA-blank-keycaps-planck-ace40-xt-Keyset-Blank-Similar-to-DSA-For-MX-Mechanical-Keyboard-Ergo/32824353605.html)

## Editing layout:

Load ```layout/contra.azerty.json``` into http://kbfirmware.com/.
Download .hex formatted firmware after you've applied your changes.

## Flashing the Pro Micro:

1. Open [QMK Toolbox](https://github.com/qmk/qmk_toolbox).
2. Select your .hex filer under “Local file” and set the Micro-controller to “atmega32u4”.
3. Select the “Auto-Flash” check box.
4. Plug your Pro Micro in to your computer, a green LED should light up on the ProMicro.
5. Use a wire to short “RST” and “GND” together on your ProMicro.
6. Remove the wire. QMK Toolbox should detect a “Caterina device” and begin the flash process. Two red LEDs should flash a number of times.
7. The red LEDs should turn off. QMK Toolbox should list “Caterina device disconnected”.
8. Unplug the ProMicro. Plug it back in. Your computer should detect it as a keyboard.
9. Short “A1” to “A2” with notepad or a similar application open. Characters should be typed.
10. If characters appear after shorting “A1” to “A2”, your Pro Micro has been flashed successfully. Let’s build!

## Reprogramming the Pro Micro:

1. Open [QMK Toolbox](https://github.com/qmk/qmk_toolbox).
2. Select your .hex filer under “Local file” and set the Micro-controller to “atmega32u4”.
3. Select the “Auto-Flash” check box.
4. Plug your USB cable in while holding down the reset switch.
5. Release the reset switch. QMK Toolbox should detect a “Caterina device” and begin the flash process. Two red LEDs should flash a number of times.
6. Remove the wire. QMK Toolbox should detect a “Caterina device” and begin the flash process. Two red LEDs should flash a number of times.
7. The red LEDs should turn off. QMK Toolbox should list “Caterina device disconnected”.
8. Unplug the ProMicro. Plug it back in. Your computer should detect it as a keyboard.
9. Your keyboard should be reprogrammed with your new layout, enjoy!
