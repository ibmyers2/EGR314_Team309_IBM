##Message Type Breakdown

Motor Direction(Type 1):

| Byte #        | Byte 1-2   | Byte 3        | Byte 4          | Byte 5-6    | Byte 7-8    |
|---------------|------------|---------------|-----------------|-------------|-------------|
| Variable Name | msgPref    | MotorD_Sender | MotorD_Reciever | MotorD_Data | msgSuf      |
| Variable Type | uint16_t   | uint_8        | uint_8          | uint16_t    | uint16_t    |
| Minimum Value | 0          | 0             | 0               | 0           | 0           |
| Maximum Value | 65535      | 255           | 255             | 65535       | 65535       |
| Example Value | 2000       | 38            | 209             | 38920       | 2005        |

Motor Rotational Velocity(Type 3):

| Byte #        | Byte 1-2   | Byte 3        | Byte 4          | Byte 5-6    | Byte 7-8    |
|---------------|------------|---------------|-----------------|-------------|-------------|
| Variable Name | msgPref    | MotorV_Sender | MotorV_Reciever | MotorV_Data | msgSuf      |
| Variable Type | uint16_t   | uint_8        | uint_8          | uint16_t    | uint16_t    |
| Minimum Value | 0          | 0             | 0               | 0           | 0           |
| Maximum Value | 65535      | 255           | 255             | 65535       | 65535       |
| Example Value | 2000       | 38            | 209             | 38920       | 2005        |

Team IDs:

| Team Member       | Set IDs |
|-------------------|---------|
| Bruce Myers       | M       |
| Baron Guido       | B       |
| Aadish Lele       | A       |
| Shaurya Manglik   | S       |
| Broadcast Message | X       |


