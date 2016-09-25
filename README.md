# uh-doc
Unofficial document for Unlimited Hand.

# Hardware

## Arduino Pins
|       Function       |       Define       |     Port    |                          Description                           |
|----------------------|--------------------|-------------|----------------------------------------------------------------|
| Vibration Motor      | vibrationMotor_PIN | digital 13  | Low: Move, High: Stop.                                         |
| Photo Reflector LED  | PR_LED_PIN         | digital 8   | Low: On, High: Off.                                            |
| Photo Reflector Recv | N/A                | analog 0-7  | Analog value.                                                  |
| Multiplexer for EMS  | EMS_S[0,1,2]_PIN   | digital 4-6 | Port selection for EMS by 3bit.                                |
| EMS                  | EMS_EN_PIN         | digital 7   | Low: Low pulse(off?), High: High pulse.                        |
| Charge for EMS?      | BOOSTER_SWITCH_PIN | digital 9   | Low: Off, High: Charge.  Charge time seems related to voltage. |

## I2C
|    IC    |        Define       | I2C addr |
|----------|---------------------|----------|
| MPU-6050 | MPU6050_I2C_ADDRESS | 0xD0     |
| SDA      | SDA_PORT            | PORTB, 2 |
| SCL      | SCL_PORT            | PORTD, 3 |
