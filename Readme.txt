Simple driver library for a MAX7219 VU style LED display board
November 2019 - David Mottram

Uses a single MAX7219 display driver chip
-----------------------------------------
	Pin connections
    Name      Arduino     MAX7219 7 Segment display
    -----     -------     -------------------------
              +5V         VCC
              GND         GND
    DIN       D11/MOSI    DIN
    CS        D10/SS      CS
    CLK       D13/SCK     CLK

  // Characters 0-F   Op-code
  0b01111110,       //  0x00 - '0'
  0b00110000,       //  0x01 - '1'
  0b01101101,       //  0x02 - '2'
  0b01111001,       //  0x03 - '3'
  0b00110011,       //  0x04 - '4'
  0b01011011,       //  0x05 - '5'
  0b01011111,       //  0x06 - '6'
  0b01110000,       //  0x07 - '7'
  0b01111111,       //  0x08 - '8'
  0b01111011,       //  0x09 - '9'
  0b01110111,       //  0x0A - 'A'
  0b00011111,       //  0x0B - 'B'
  0b01001110,       //  0x0C - 'C'
  0b00111101,       //  0x0D - 'D'
  0b01001111,       //  0x0E - 'E'
  0b01000111,       //  0x0F - 'F'

  // Other Characters
  0b00000001,       //  0x10 - '- minus'
  0b01000011,       //  0x11 - 'c for centigrade'
  0b01100011,       //  0x12 - 'o for degree'
  0b00110111,       //  0x13 - 'H'
  0b00001110,       //  0x14 - 'L'
  0b01110110,       //  0x15 - 'n'
  0b01100111,       //  0x16 - 'P'
  0b00001111,       //  0x17 - 't'
  0b00111011,       //  0x18 - 'Y'
  0b00111110,       //  0x19 - 'U'
  0b00000101,       //  0x1A - 'r'
  
  0b00000000        //  0x1B - 'blank'
