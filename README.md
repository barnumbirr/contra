

# contra
Everything I need for my [Contra 40% ortholinear keyboard](https://cartel.ltd/projects/contra).

## Parts

```coming soon```

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

<img src="https://raw.githubusercontent.com/mrsmn/contra/master/images/flash_1.png" height=256>
<img src="https://raw.githubusercontent.com/mrsmn/contra/master/images/flash_2.png" height=256>

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
