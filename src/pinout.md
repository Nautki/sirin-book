# Pinout
## Exposed GPIO Pins

Every exposed pin can be used as GPIO or as an interrupt. In addition to those two roles, certain pins can also be used for other alternative functions (AF), as detailed in the table below. Unusable/useless AFs have been omitted.

| SirinS1 | STM32 | AF | AF | AF | AF |
|---------|-------|--------------|-|-|-|
|  1 |  PA4 | DAC_OUT1 | D1PWREN | TIM5_ETR
|  2 |  PC4 | ADC1_INP4
|  3 |  PC5 | ADC1_INN4 | COMP1_OUT
|  4 |  PB0 | ADC1_INN5
|  5 |  PB1 | ADC1_INP5
|  6 |  PB2 | QUADSPI_CK | SPI3_MOSI/I2S3_SDO | RTC_OUT
|  7 |  PE7 | QUADSPI_BK2_IO0 | UART7_RX | TIM1_ETR
|  8 |  PE8 | QUADSPI_BK2_IO1 | UART7_TX | TIM1_CH1N | COMP2_OUT
|  9 |  PE9 | QUADSPI_BK2_IO2 | UART7_RTS/UART7_DE | TIM1_CH1
| 10 | PE10 | QUADSPI_BK2_IO3 | UART7_CTS | TIM1_CH2N
| 11 |  PD7 | USART2_CK
| 12 |  PD6 | USART2_RX | SPI3_MOSI/IS2S3_SDO
| 13 |  PD5 | USART2_TX
| 14 |  PD4 | USART2_RTS/USART2_DE
| 15 |  PD3 | USART2_CTS/USART2_NSS
| 16 |  PD1 | FDCAN1_TX | UART4_TX

Pins 17-20 are connected to MOSFETs:

| Pin | Wiring | Connected to |
|----|-----|-----|
| 17 | Q2- | GND |
| 18 | Q2+ |     |
| 19 | Q1- | GND |
| 20 | Q1+ |     |

On SirinS1-R1, the wiring was:

| SirinS1 | STM32 | AF | AF | AF | AF |
|---------|-------|----|----|----|----|
| 17 |  PD0 | FDCAN1_RX | UART4_RX
| 18 | PC12 | SPI3_MOSI/I2S3_SDO | USART3_CK
| 19 | PC11 | SPI3_MISO/I2S3_SDI | USART3_RX | UART4_RX
| 20 | PC10 | SPI3_SCK/I2S3_CK | USART3_TX | UART4_TX