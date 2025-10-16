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
# Modificando de Si4825 para Si4827 com interface Digital

## Slide 1

### Converting a low-cost radio based on the Si4825 into a digital interface radio using the Si4827.

![Slide 1 image](converted/images/slide1_img_1.jpg)

![Slide 1 image](converted/images/slide1_img_2.jpg)

---

## Slide 2

### About the low-cost radio (KapBom K2019)

- Two bands (MW and FM)

- Less than $5

- Compact and lightweight

- Based on the Si4825 DSP

- Sturdy plastic casing

- Analog interface

![Slide 2 image](converted/images/slide2_img_3.jpg)

- Warning: There are other receivers from different manufacturers that use the same casing but are not

- equipped with the Si4825. Be sure the receiver is equipped with the Si4825.

---

## Slide 3

### About the modified radio

- 15 bands (3 FM, 2 AM, and 10 SW)

- Bands can be configured via programming

- Based on the Si4827 DSP

- Uses the Seeeduino XIAO controller (ARM Cortex-M0+)

![Slide 3 image](converted/images/slide3_img_4.jpg)

---

## Slide 4

### Components used for the modification

![Slide 4 image](converted/images/slide4_img_5.jpg)

![Slide 4 image](converted/images/slide4_img_6.jpg)

![Slide 4 image](converted/images/slide4_img_7.jpg)

- SEEEDUINO XIAO

- ARM Cortex-M0+

![Slide 4 image](converted/images/slide4_img_8.jpg)

OLED I2C

SI 4827

Push Buttons

---

## Slide 5

### About the DSP Si4825

![Slide 5 image](converted/images/slide5_img_9.png)

- Support for FM band (64–109 MHz)

- Support for AM band (504–1750 kHz)

- Support for SW band (2.3–28.5 MHz)

- No manual calibration required

- Mono audio output

- Band configuration according to region (AM/FM/SW)

- Enhanced coverage for FM/SW bands

---

## Slide 6

### About the  DSP Si4827

![Slide 6 image](converted/images/slide6_img_10.png)

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

## Slide 7

### Open radio (before modification)

![Slide 7 image](converted/images/slide7_img_11.jpg)

---

## Slide 8

### Board (before modification)

![Slide 8 image](converted/images/slide8_img_12.jpg)

![Slide 8 image](converted/images/slide8_img_13.jpg)

---

## Slide 9

### Si4825 Identification (Check if the radio is based on Si4825)

![Slide 9 image](converted/images/slide9_img_14.jpg)

![Slide 9 image](converted/images/slide9_img_15.png)

---

## Slide 10

### Replacement of Si4825 with Si4827

![Slide 10 image](converted/images/slide10_img_16.jpg)

![Slide 10 image](converted/images/slide10_img_17.jpg)

---

## Slide 11

### Si4827 soldered on the board

![Slide 11 image](converted/images/slide11_img_18.jpg)

![Slide 11 image](converted/images/slide11_img_19.jpg)

---

## Slide 12

### Si4827 with a cut on the trace leading to pin 4 (BAND)

![Slide 12 image](converted/images/slide12_img_20.jpg)

---

## Slide 13

### Si4827 and Seeduino XIAO wireup

- | SI4827 pin | SEEEDUINO pin |  Description                |

- | ---------  | ------------  | ----------------------------|

- |    1       |  2            | SEEEDUINO interrupt pin     |

- |    9       |  6            | RESET                       |

- |   10       |  A4 (SDA)     | I2C bus (Data)              |

- |   11       |  A5 (SCL)     | I2C bus (Clock)             |

- | -----------| ------------- | ----------------------------|

- |  OLED      |               |                             |

- | -----------| ------------- | ----------------------------|

- |   SDA      |  4            | I2C Bus (Data)              |

- |   CLK      |  5            | I2C bus (CLock)             |

- | -----------| ------------- | ----------------------------|

- |Push Buttons|               |                             |

- | -----------| ------------- | ----------------------------|

- |  BAND UP   |  7            | Next Band.                  |

- |  BAND DOWN |  8            | Previous Band               |

---

## Slide 14

### Checking the Si4827 and Seeduino XIAO setup

![Slide 14 image](converted/images/slide14_img_21.png)

---

## Slide 15

### Case modification

![Slide 15 image](converted/images/slide15_img_22.jpg)

![Slide 15 image](converted/images/slide15_img_23.jpg)

---

## Slide 16

### Case modification

![Slide 16 image](converted/images/slide16_img_24.jpg)

---

## Slide 17

### Finish

![Slide 17 image](converted/images/slide17_img_25.jpg)

---
