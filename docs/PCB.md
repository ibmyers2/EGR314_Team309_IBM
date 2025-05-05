## PCB

![Image](https://github.com/user-attachments/assets/eaf92b7a-6e61-49a3-8893-2047c0ab426c)

![Image](https://github.com/user-attachments/assets/27574fa5-7a6a-4a54-8ad9-aae2a54519c1)

![Image](https://github.com/user-attachments/assets/616fc9be-8d91-498f-8d6a-661c5ab04f68)

![Image](https://github.com/user-attachments/assets/4a30c898-1568-4b90-bd71-6bcebda43b32)

[Gerber Files](https://github.com/user-attachments/files/20048113/Myers_Updated_Board.zip)

## PCB Decision Making Process
When it came to making the layout of the PCB, I wanted to make the layout fairly compact, but since the HMI would be a stand-alone part of the project, I did have more freedom to make more space. Aside from ensuring that there was enough space to be able to push down on push buttons and to solder components, I was able to make a stable board with little restriction. Aside from facing my barrel jack the wrong direction and some issues with importing the USB programmer onto the wrong layer of the board, this PCB design worked well for the project and was very neat and organized.

## Version 2.0 Potential Improvements
As far as creating a version 2.0 of this human machine interface, there are a couple of changes that I would be sure to make. One of these would be to make sure to check that all parts had been placed properly before sending out the design for manufacturing. In this design, my USB had been placed upside down onto the bottom of the board, which confused me when trying to assemble the components onto the board to begin testing. The barrel jack is also facing in the direction of one of the ribbon cable headers, which means it could be soldered on, but not connected, since the headers would be in the way. Small issues like these made the board harder to assemble and understand, so taking more time to ensure parts are placed properly would be a huge improvement in another iteration. I would also make sure to try and keep all of the passive components the same pad size. This would allow for more freedom if certain parts didn’t function as expected. This happened with the voltage regulator circuit, which caused issues close to the final deadline for the project. The final change I would make to the PCB design would be to consider where headers would need to be placed and add more space between these areas. This was an issue with the push buttons when I attempted to place the system into the 3D printed case for the human machine interface.
