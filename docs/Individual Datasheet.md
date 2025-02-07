##Components

-ESP32 Microcontroller

-Voltage Regulator (3.3V)

-Pushbutton

-OLED Screen

-9V 1A Battery Power Supply

Block Diagram:

![Image](https://github.com/user-attachments/assets/3f3b6a4d-3d0d-42b7-96c4-5cf76b788ec1)

##Component Selection

OLED Screen:

| Potential Solution                                                                                                                                                                                                              | Pros                                                                                                 | Cons                                                   |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------|--------------------------------------------------------|
| <br>AOM12864A0-1.54WW<br>[Digikey Link](https://www.digikey.com/en/products/detail/orient-display/AOM12864A0-1-54WW/22531841)<br>![Image](https://github.com/user-attachments/assets/706e427e-557f-4cc8-b491-9308bc0a0bee)      | -$17.60<br>-I2C Compatible communication<br>-Lightweight, 1.5-inch screen size<br>-Max 45 mA current | -15V required for display                              |
| NHD-1.8-160128UBC3<br>[Digikey Link](https://www.digikey.com/en/products/detail/newhaven-display-intl/NHD-1-8-160128UBC3/23334148)<br>![Image](https://github.com/user-attachments/assets/69c1b4db-8b82-407b-85b5-7c32fe665202) | -3.3V max power<br>-Lightweight, 1.8 inch screen size                                                | -200-250 mA current<br>-$25.91<br>-Not I2C Compattable |
|                                                                                                                                                                                                                                 |                                                                                                      |                                                        |

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

