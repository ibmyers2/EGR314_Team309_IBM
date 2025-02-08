##Component Selection

OLED Screen:

| Potential Solution                                                                                                                                                                                                                                                                                                      | Pros                                                                                                 | Cons                                                  |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------|-------------------------------------------------------|
| AOM12864A0-1.54WW<br>[Digikey Link](https://www.digikey.com/en/products/detail/orient-display/AOM12864A0-1-54WW/22531841)<br>![Image](https://github.com/user-attachments/assets/706e427e-557f-4cc8-b491-9308bc0a0bee)                                                                                                  | -$17.60<br>-I2C Compatible communication<br>-Lightweight, 1.5-inch screen size<br>-Max 45 mA current | -15V required for display                             |
| NHD-1.8-160128UBC3<br>[Digikey Link](https://www.digikey.com/en/products/detail/newhaven-display-intl/NHD-1-8-160128UBC3/23334148)<br>![Image](https://github.com/user-attachments/assets/69c1b4db-8b82-407b-85b5-7c32fe665202)                                                                                         | -3.3V max power<br>-Lightweight, 1.8-inch screen size                                                | -200-250 mA current<br>-$25.91<br>-Not I2C Compatible |
| Teyleten Robot 0.96 inch LCD OLED Display Board Module 12864 128X64 IIC I2C SSD1306 Driver 4 Pins for Raspberry Pi Arduino<br>[Amazon Link](https://www.amazon.com/Teyleten-Robot-Display-SSD1306-Raspberry/dp/B0CN373JF4)<br>![Image](https://github.com/user-attachments/assets/7bb9008b-2bfa-4ad3-878a-faf646474335) | -I2C compatible<br>-$12.88 for 5<br>-3V-5V<br>-Low power rating                                      | -Smaller screen                                       |

Optimal Solution: Teyleten Robot 0.96 inch LCD OLED Display Board Module 12864 128X64 IIC I2C SSD1306 Driver 4 Pins for Raspberry Pi Arduino

Rationale: While smaller than the others, this screen will be very affordable and can be replaced easily if something is not done properly. It also is compatible with the other components in the system. The information that we will need to display should fit on the screen, so this screen will be optimal for the system.

3.3V Voltage Regulator:

| Potential Solution                                                                                                                                                                                                          | Pros                                                                                | Cons                                            |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------|-------------------------------------------------|
| LMR50410Y3FQDBVRQ1<br>[Digikey Link](https://www.digikey.com/en/products/detail/texas-instruments/LMR50410Y3FQDBVRQ1/13562985)<br>![Image](https://github.com/user-attachments/assets/15f5f066-986a-48c2-af60-6b1341b0c69d) | -Smaller in size<br>-Less pins<br>-38 V Max Input<br>-1A output<br>-$1.47           | -Closer pins, may make soldering more difficult |
| LM2575-3.3WU-TR<br>[Digikey Link](https://www.digikey.com/en/products/detail/microchip-technology/LM2575-3-3WU-TR/1027646)<br>![Image](https://github.com/user-attachments/assets/ae5945d1-fce3-4625-ad35-fdb6e194ff74)     | -$1.75<br>-40V Input<br>-1A Output<br>-All pins on 1 side, easier to design for PCB | -Closer pins, may be difficult to solder        |
| LM2675MX-3.3/NOPB<br>[Digikey Link](https://www.digikey.com/en/products/detail/texas-instruments/LM2675MX-3-3-NOPB/366907)<br>![Image](https://github.com/user-attachments/assets/dfdbf7d2-0463-4921-9ae8-ce323a9c8bc2)     | -45V Input<br>-1A Output<br>-Easier to solder                                       | -$4.36<br>-More pins                            |

Optimal Solution: LM2675MX-3.3/NOPB

Rationale: While more expensive, this voltage regulator will be easier to solder than the other much smaller components with more difficult pins. This will also allow for more room for traces on the PCB. It has a well-within-range voltage requirement and enough amperage for the system.

Power Supply:

| Potential Solution                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  | Pros                                                                                               | Cons                                                                                                         |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------|
| WR9HD1333CCP-F(R6B)<br>[Digikey Link](https://www.digikey.com/en/products/detail/globtek-inc/WR9HD1333CCP-F(R6B)/13245472?gclsrc=aw.ds&&utm_adgroup=General&utm_source=google&utm_medium=cpc&utm_campaign=PMax%20Shopping_Product_Zombie%20SKUs&utm_term=&utm_content=General&utm_id=go_cmp-17815035045_adg-_ad-__dev-c_ext-_prd-13245472_sig-CjwKCAiA2JG9BhAuEiwAH_zf3iB5fHK3lgCYxPQfWTUMx6az-ZwQjhctqcc9AtKmA3itkMB3NoGBfxoC30cQAvD_BwE&gad_source=1&gclid=CjwKCAiA2JG9BhAuEiwAH_zf3iB5fHK3lgCYxPQfWTUMx6az-ZwQjhctqcc9AtKmA3itkMB3NoGBfxoC30cQAvD_BwE&gclsrc=aw.ds)<br>![Image](https://github.com/user-attachments/assets/1f13eba8-3f1b-40f7-a6e3-9435a75f3d95) | -$3.94<br>-9V Output<br>-1.33 A Output<br>-Barrel Jack cord                                        | -Wall-connected<br>-Cord must reach into subsystem to power                                                  |
| 1300mAh High Capacity Lithium-ion Long Lasting 9 Volt Batteries<br>[Amazon Link](https://www.amazon.com/PAISUE-Rechargeable-Lithium-ion-Multimeter-Microphone/dp/B0B248DSFG?source=ps-sl-shoppingads-lpcontext&ref_=fplfs&smid=A2WEVNKRB72JGE&gQT=1&th=1)<br>![Image](https://github.com/user-attachments/assets/1379a413-64ab-420f-8771-392321a2b992)                                                                                                                                                                                                                                                                                                              | -Portable<br>-9V Output<br>-1.3A Output<br>-Can be incorporated into the system for no outer cords | -$11.98 (for 2)<br>-Ships quickly through Amazon<br>-No build-in connector                                   |
| 9 Volt DC, 1 Amp Power Adapter with 5.5mm Barrel Jack, 2.1mm Inner Diameter<br>[Elexp Link](https://www.elexp.com/products/16d9-1wall-adaptor-9v-1a-plug-2-1mm?variant=42666546102500&currency=USD&utm_source=google&utm_medium=organic&utm_campaign=Google%20Shopping&utm_content=9%20Volt%20DC%2C%201%20Amp%20Power%20Adapter%20with%205.5mm%20Barrel%20Jack%2C%202.1mm%20Inner%20Diameter%20(Center%20Positive)&gad_source=1&gclid=CjwKCAiA2JG9BhAuEiwAH_zf3kCQT20F8pNUSFtNsfVa0HCrzU7W_4cg6pAwINuGU1AnPQ9iI671IBoC5IsQAvD_BwE)<br>![Image](https://github.com/user-attachments/assets/5c68a02f-8b00-4066-8371-12162a3a0a00)                                     | -Barrel Jack Connector<br>-9V Output<br>-1.3A Output                                               | -$5.95<br>-Not shipped through Digikey/Amazon<br>-Wall Connected<br>-Cord must reach into subsystem to power |

Optimal Solution: 1300mAh High Capacity Lithium-ion Long Lasting 9 Volt Batteries

Rationale: The Portable battery that is shown would be the best option of the three because our presentation for the Innovation showcase will be made significantly smoother with the use of a portable power supply. We will not have to worry about cords outside of the system, as we can make a shell and have the battery and barrel jack adapter built within the system. We can also purchase only a few packs of these and can recharge them for multiple uses, which is better than buying many batteries.

Microcontroller Selection

Requirements:
-1 I2C communication pin
-2 UART communication pins
-Multiple GPIO pins

First Microcontroller consideration: ESP32-S3-WROOM-1-N4

| ESP Info                                | Answer                                                                                                                                                                                                 |
|-----------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Model                                   | ESP32-S3-WROOM-1-N4                                                                                                                                                                                    |
| Product Page URL                        | [Digikey Link](https://www.digikey.com/en/products/detail/espressif-systems/ESP32-S3-WROOM-1-N4/16162639)                                                                                              |
| ESP32-S3-WROOM-1-N4 Datasheet URL       | [ESP32-S3-WROOM-1-N4 Datasheet Link](https://www.espressif.com/sites/default/files/documentation/esp32-s3-wroom-1_wroom-1u_datasheet_en.pdf)                                                           |
| ESP32 S3 Datasheet URL                  | [ESP32 S3 Datasheet](https://www.espressif.com/sites/default/files/documentation/esp32-s3_datasheet_en.pdf)                                                                                            |
| ESP32 S3 Technical Reference Manual URL | [ESP32 S3 Technical Reference Manual](https://www.espressif.com/sites/default/files/documentation/esp32-s3_technical_reference_manual_en.pdf)                                                          |
| Vendor Link                             | [Espressif Systems Link](https://www.digikey.com/en/supplier-centers/espressif-systems)                                                                                                                |
| Code Examples                           | [Code Examples](https://github.com/espressif/arduino-esp32/blob/master/libraries/WiFi/examples/SimpleWiFiServer/SimpleWiFiServer.ino)                                                                  |
| External resources URL(s)               | [Getting started with ESP32](https://www.youtube.com/watch?v=UuxBfKA3U5M&pp=ygUOZXNwMzIgdHV0b3JpYWw%3D)<br>[ESP32 Overview](https://www.youtube.com/watch?v=QUNKY87Da7A&pp=ygUOZXNwMzIgdHV0b3JpYWw%3D) |
| Unit Cost                               | $2.95                                                                                                                                                                                                  |
| Absolute Maximum Current for entire IC  | 0.5A                                                                                                                                                                                                   |
| Supply Voltage Range                    | 3.0-3.6V                                                                                                                                                                                               |
| Maximum GPIO current (per pin)          | 10nA                                                                                                                                                                                                   |
| Support External Interrupts?            | Yes                                                                                                                                                                                                    |
| Require Programming Hardware, Cost, URL | None                                                                                                                                                                                                   |

Highlights: The ESP32 will be able to do more than enough for the system that needs to be created. There is an array of GPIO pins that also work as I2C pins, so there is little need to worry about the OLED’s positioning. These GPIO pins also work well with the pushbuttons that may need to be used. The required current is also half of what will be accessible, which leaves another 0.5A for the other components. This microcontroller also has the proper UART communication that is needed for using Wifi to establish communication between the human interface and other systems.

Pin Info:

![Image](https://github.com/user-attachments/assets/f78ca74e-7bdd-41c8-8a52-8aa312c4e7d6)
![Image](https://github.com/user-attachments/assets/26f5d32e-5a77-4e69-86b7-409646a7729f)
![Image](https://github.com/user-attachments/assets/a7af341e-1e53-413c-abfa-90c2efcc2912)
![Image](https://github.com/user-attachments/assets/007f67ed-6521-49e2-baa5-ee6ff3953eca)

Team Role:

As the member of the team that is responsible for the human interface system, I will have a few primary responsibilities. The first of these is going to be making sure my system is powered. Since it will be its standalone system compared to to spinning top, which will have the actuator, sensor, etc, I will be in charge of making sure that the human interface is powered at all times. I will also be responsible for the display. This will be what allows us to have a great exhibit that can be properly interacted with by the visitors at the showcase. Finally, I will also be in charge of establishing communication between the spinning top using Wifi capabilities. This is what will allow my system to receive the speed data and possibly send out data to control the top.

| Module         | # Available | Needed | Associated Pins                                                    |
|----------------|-------------|--------|--------------------------------------------------------------------|
| UART           | 24          | 2      | Any GPIO Pins(4-12,15-31)(Pins 36 and 37 specially designated)     |
| SPI            | 24          | 0      | Any GPIO Pin(4-12,15-31)(depends on what peripheral is being used) |
| I2C            | 24          | 1      | Any GPIO Pin(4-12,15-31)                                           |
| GPIO           | 24          | 2      | Any GPIO Pin(4-12,15-31)                                           |
| ADC            | 3           | 0      | 13, 14, and 18                                                     |
| LED PWM        | 24          | 0      | Any GPIO Pin(4-12,15-31)                                           |
| Motor PWM      | 24          | 0      | Any GPIO Pin(4-12,15-31)                                           |
| USB Programmer | 2           | 1      | 13 and 14 (GPIO19 and 20)                                          |

Conclusion:

Overall, the ESP32 works wonderfully as a microcontroller for my system. It fulfills the project requirement and has many functions that work well with my goals and ideas. It has all the compatible systems needed for my peripherals, including I2C, UART, and GPIO pins. It also has many of these pins available, so worrying about where on the board to place components should not be too much of a problem. The ESP32 also has a low current requirement and only needs a voltage regulator to be powered. It also comes with an antenna, so no additional hardware will be required.
