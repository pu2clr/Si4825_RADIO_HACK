# Converting Si4825 to Si4827 with Digital Interface

## Slide 1

### Converting a low-cost radio based on the Si4825 into a digital interface radio using the Si4827.

![Slide 1 image](images/slide1_img_1.jpg)
![Slide 1 image](images/slide1_img_2.jpg)

---

## Slide 2 — About the low-cost radio (KapBom K2019)

- Two bands (MW and FM)
- Less than $5
- Compact and lightweight
- Based on the Si4825 DSP
- Sturdy plastic casing
- Analog interface

![](images/slide2_img_3.jpg)

- Warning: There are other receivers from different manufacturers that use the same casing but are not equipped with the Si4825. Be sure the receiver is equipped with the Si4825.

---

## Slide 3 — About the modified radio

- 15 bands (3 FM, 2 AM, and 10 SW)
- Bands can be configured via programming
- Based on the Si4827 DSP
- Uses the Seeeduino XIAO controller (ARM Cortex-M0+)

![](images/slide3_img_4.jpg)

---

## Slide 4 — Components used for the modification

![](images/slide4_img_5.jpg)
![](images/slide4_img_6.jpg)
![](images/slide4_img_7.jpg)

- Seeeduino XIAO (ARM Cortex-M0+)
- OLED (I2C)
- Si4827
- Push Buttons

![](images/slide4_img_8.jpg)

---

## Slide 5 — About the DSP Si4825

![](images/slide5_img_9.png)

- Support for FM band (64–109 MHz)
- Support for AM band (504–1750 kHz)
- Support for SW band (2.3–28.5 MHz)
- No manual calibration required
- Mono audio output
- Band configuration according to region (AM/FM/SW)
- Enhanced coverage for FM/SW bands

---

## Slide 6 — About the DSP Si4827

![](images/slide6_img_10.png)

- Support for FM band (64–109 MHz)
- Support for AM band (504–1750 kHz)
- Support for SW band (2.3–28.5 MHz)
- Selectable support for all regional AM/FM/SW bands
- Enhanced coverage of FM/SW bands
- 2-wire control interface (I2C)
- Valid station indicator
- Support for digital volume control
- Support for bass and treble adjustment

---

## Slides 7–12 — Disassembly, board, replacement, and photos

These slides show the radio opened, the board before modification, identification of the Si4825, replacement steps, and photos of the Si4827 soldered and the trace cut on pin 4 (BAND).

![](images/slide7_img_11.jpg)
![](images/slide8_img_12.jpg)
![](images/slide8_img_13.jpg)
![](images/slide9_img_14.jpg)
![](images/slide9_img_15.png)
![](images/slide10_img_16.jpg)
![](images/slide10_img_17.jpg)
![](images/slide11_img_18.jpg)
![](images/slide11_img_19.jpg)
![](images/slide12_img_20.jpg)

---

## Slide 13 — Wiring (Si4827 and Seeeduino XIAO)

| Si4827 pin | Seeeduino pin | Description            |
|------------|---------------|------------------------|
| 1          | 2             | Seeeduino interrupt pin|
| 9          | 6             | RESET                  |
| 10         | A4 (SDA)      | I2C bus (Data)         |
| 11         | A5 (SCL)      | I2C bus (Clock)        |

### OLED wiring

| OLED pin | Seeeduino pin | Description     |
|----------|---------------|-----------------|
| SDA      | 4             | I2C Bus (Data)  |
| CLK      | 5             | I2C Bus (Clock) |

### Push buttons wiring

| Button    | Seeeduino pin | Function       |
|-----------|---------------|----------------|
| BAND UP   | 7             | Next Band      |
| BAND DOWN | 8             | Previous Band  |

---

## Slide 14 — Checking the Si4827 and Seeeduino XIAO setup

![](images/slide14_img_21.png)

---

## Slides 15–16 — Case modification

![](images/slide15_img_22.jpg)
![](images/slide15_img_23.jpg)
![](images/slide16_img_24.jpg)

---

## Slide 17 — Finish

![](images/slide17_img_25.jpg)

---
