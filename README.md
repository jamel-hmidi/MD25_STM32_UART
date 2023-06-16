UART Communication between an MD25 Motor Driver and STM32F407:
Controlling the EMG30 motors speed using a potentiometer

Steps:
- Enable the USART4 (or any other UART interface) in asynchrounous mode.
- Choose the appropriate Baud Rate as the hardware configuration of the MD25 (See MD25 Documentation)
- No parity, 2 Stop Bits
- In USART4 NVIC Settings, enable the global interrupt
- In DMA Settings, add the UART4_RX DMA Request
- Enable one ADC Input (Potentiometer Input)

Components:
- STM32F407
- MD25 Motor Driver
- Two EMG30 Motors
- Potentiometer
- 12V Charger


MD25 Documentation Link: http://www.robot-electronics.co.uk/htm/md25tech.htm