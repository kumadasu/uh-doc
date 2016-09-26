# uh-doc
Unofficial document for Unlimited Hand.

# Hardware

## Arduino Pins
|       Function       |       Define       |  Port |                          Description                           |
|----------------------|--------------------|-------|----------------------------------------------------------------|
| Multiplexer for EMS  | EMS_S[0,1,2]_PIN   | D4-D6 | Port selection for EMS by 3bit.                                |
| EMS                  | EMS_EN_PIN         | D7    | Low: Low pulse(off?), High: High pulse.                        |
| Photo Reflector LED  | PR_LED_PIN         | D8    | Low: On, High: Off.                                            |
| Charge for EMS?      | BOOSTER_SWITCH_PIN | D9    | Low: Off, High: Charge.  Charge time seems related to voltage. |
| Vibration Motor      | vibrationMotor_PIN | D13   | Low: Move, High: Stop.                                         |
| Photo Reflector Recv | N/A                | A0-A7 | Analog value.                                                  |

## I2C
|    IC    |        Define       | I2C addr |
|----------|---------------------|----------|
| MPU-6050 | MPU6050_I2C_ADDRESS | 0xD0     |
| SDA      | SDA_PORT            | PORTB, 2 |
| SCL      | SCL_PORT            | PORTD, 3 |
