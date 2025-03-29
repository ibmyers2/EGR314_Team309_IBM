##Message Type Breakdown

Motor Direction(Type 1):

| Byte #        | Byte 1-2   | Byte 3        | Byte 4          | Byte 5-6    | Byte 7-8    |
|---------------|------------|---------------|-----------------|-------------|-------------|
| Variable Name | msgPref    | MotorD_Sender | MotorD_Reciever | MotorD_Data | msgSuf      |
| Variable Type | uint16_t   | uint_8        | uint_8          | uint16_t    | uint16_t    |
| Minimum Value | AZ         | M             | A               | 0x0040      | YB          |
| Maximum Value | AZ         | M             | A               | 0x0041      | YB          |
| Example Value | AZ         | M             | A               | 0x0040      | YB          |

Motor Rotational Velocity(Type 3):

| Byte #        | Byte 1-2   | Byte 3        | Byte 4          | Byte 5-6    | Byte 7-8    |
|---------------|------------|---------------|-----------------|-------------|-------------|
| Variable Name | msgPref    | MotorV_Sender | MotorV_Reciever | MotorV_Data | msgSuf      |
| Variable Type | uint16_t   | uint_8        | uint_8          | uint16_t    | uint16_t    |
| Minimum Value | AZ         | S             | M               | 0           | YB          |
| Maximum Value | AZ         | S             | M               | 65535       | YB          |
| Example Value | AZ         | S             | M               | 38920       | YB          |

Team IDs:

| Team Member       | Set IDs |
|-------------------|---------|
| Bruce Myers       | M       |
| Baron Guido       | B       |
| Aadish Lele       | A       |
| Shaurya Manglik   | S       |
| Broadcast Message | X       |


