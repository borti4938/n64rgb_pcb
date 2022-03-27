
### Jumpers N64RGBv1

- J11.1 -> activates 15bit color mode if closed.  **[1]**
- J11.2 -> activates VI-deblur if closed. **[1]**
  - J11.x are just pins on older versions. J11.1 is pin 91 (short to pin 90 to close jumper) and J11.2 is pin 2 (short to pin 1 to close jumper) **[2]**
- Pin 36 -> disables IGR functions toggle deblur and 15bit mode if shorted to pin 37 **[2]**
- J12 -> disables IGR function reset by controller
  - is just pin 66 on older v1 boards without a jumper - short to pin 67 to close jumper **[2]**
- Pad _FIL_ -> einables SD filter from THS7374 if open and disables filter if shorted to GND
  - on older boards it is pin 85 (unfortunately there is no GND pin next to it, so you have to short it with a wire to GND if you need to disable the SD filter)


### Jumpers N64RGBv2

- J11.1 -> activates 15bit color mode if closed.  **[1]**
- J11.2 -> activates VI-deblur if closed. **[1]**
- J12.x -> disables IGR functions if closed
  - x.1: VI-DeBlur and 15bit mode toggle by controller
  - x.2: reset by controller
- J21 -> enables Sync on Green if closed

### Notes  

All pins referring to pins of the CPLD (U1).

**[1]**  
Jumper becomes active on power cycle or if toggled while running operation.  

**[2]**
These are 'hidden jumper', which means it is just a pin where the neighbored pin is GND.

