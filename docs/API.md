##Message Type Breakdown

Toggle Motor(Type 1):

| Byte #        | Byte 1-2   | Byte 3        | Byte 4          | Byte 5-6    | Byte 7-8    |
|---------------|------------|---------------|-----------------|-------------|-------------|
| Variable Name | msgPref    | MotorD_Sender | MotorD_Reciever | Motor_Data  | msgSuf      |
| Variable Type | uint16_t   | uint_8        | uint_8          | uint16_t    | uint16_t    |
| Minimum Value | AZ         | M             | B               | 0x0040      | YB          |
| Maximum Value | AZ         | M             | B               | 0x0041      | YB          |
| Example Value | AZ         | M             | B               | 0x0040      | YB          |

Team IDs:

| Team Member       | Set IDs |
|-------------------|---------|
| Bruce Myers       | M       |
| Baron Guido       | B       |


