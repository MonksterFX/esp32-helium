# esp32 helium project

Project is derived from: https://github.com/helium/longfi-arduino/tree/master/TTGO-TBeam-Tracker

## status of project

Currently in experimental status. Works with TTGO T3 V1, 868MHZ EU frequency. 

## credentials (important)

Create a credentials file `main->credentials.h` with the following content. Replace the keys with your own keys from the helium console.

```c++
#pragma once

// for now it is need for other parts of the program
#define USE_OTAA

// APPEUI and DEVEUI must be in little-endian format, least significant bit (lsb).
static const u1_t PROGMEM APPEUI[8]  = { 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00 };
static u1_t PROGMEM DEVEUI[8]  = { 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00 };

// APPKEY must be in most-significant-bit (msb)
static const u1_t PROGMEM APPKEY[16] = { 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00 };
```




