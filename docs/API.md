##Message Type Breakdown

Motor Direction(Type 1):

| Byte #        | Byte 1     | Byte 2     | Byte 3        | Byte 4          | Byte 5      | Byte 6      | Byte 7     | Byte 8     |
|---------------|------------|------------|---------------|-----------------|-------------|-------------|------------|------------|
| Variable Name | msgPref    | msgPref    | MotorD_Sender | MotorD_Reciever | MotorD_Data | MotorD_Data | msgSuf     | msgSuf     |
| Variable Type | uint16_t   | uint16_t   | uint_8        | uint_8          | uint16_t    | uint16_t    | uint16_t   | uint16_t   |
| Minimum Value | 0          | 0          | 0             | 0               | 0           | 0           | 0          | 0          |
| Maximum Value | 65535      | 65535      | 255           | 255             | 65535       | 65535       | 65535      | 65535      |
| Example Value | 2000       | 8450       | 38            | 209             | 38920       | 2005        | 39472      | 393        |

Motor Rotational Velocity(Type 3):

| Byte #        | Byte 1     | Byte 2     | Byte 3        | Byte 4          | Byte 5      | Byte 6      | Byte 7     | Byte 8     |
|---------------|------------|------------|---------------|-----------------|-------------|-------------|------------|------------|
| Variable Name | msgPref    | msgPref    | MotorV_Sender | MotorV_Reciever | MotorV_Data | MotorV_Data | msgSuf     | msgSuf     |
| Variable Type | uint16_t   | uint16_t   | uint_8        | uint_8          | uint16_t    | uint16_t    | uint16_t   | uint16_t   |
| Minimum Value | 0          | 0          | 0             | 0               | 0           | 0           | 0          | 0          |
| Maximum Value | 65535      | 65535      | 255           | 255             | 65535       | 65535       | 65535      | 65535      |
| Example Value | 358        | 20040      | 97            | 155             | 10389       | 29876       | 394        | 63823      |
