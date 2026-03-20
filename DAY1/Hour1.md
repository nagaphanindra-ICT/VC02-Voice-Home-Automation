# Day 1 – Hour 1 (10:00 PM – 11:00 PM)

## Objective
To start the marathon development and understand the VC02 module and project concept.

## Work Done
- Started 12-hour marathon development
- Finalized project: VoiceNest (Voice Controlled Home Automation using VC02)
- Studied VC02 official datasheet

## Technical Understanding
- VC02 is an offline voice recognition module
- Supports multiple voice commands
- Works on 3.6V–5V power supply
- Provides GPIO pins to control external devices

## Learning
- VC02 can directly control appliances using relay
- No internet required (offline system)
- Suitable for smart home automation

## VC02 Architecture Diagram

                ┌───────────┬───────────┬───────────┐
                │   Power   │   RESET   │    PLL    │
                └───────────┴───────────┴───────────┘

      ┌──────────┐
      │  AMic    │
      ├──────────┤
      │  DMic    │
      ├──────────┤
      │   DAC    │
      ├──────────┤
      │ I2S I/O  │
      └──────────┘

                 ┌──────────────────────────┐
                 │          RISC            │
                 │  ┌──────┬──────┬──────┐ │
                 │  │ DSP  │ FPU  │ FFT  │ │
                 │  └──────┴──────┴──────┘ │
                 │          DMA            │
                 └──────────────────────────┘

           ┌───────────────┬───────────────┐
           │     SRAM      │     FLASH     │
           └───────────────┴───────────────┘

      ┌──────────┐
      │   GPIO   │
      ├──────────┤
      │   UART   │
      ├──────────┤
      │   I2C    │
      ├──────────┤
      │   PWM    │
      ├──────────┤
      │   SPI    │
      └──────────┘

## Understanding from Architecture
- VC02 uses a RISC processor for processing voice commands
- DSP, FPU, and FFT units help in speech recognition
- GPIO pins are used to control external devices like relays
- Communication interfaces include UART, I2C, SPI
- Internal memory (SRAM, Flash) is used for storing commands and processing data

## VC02 Architecture Understanding

The VC02 module is built with a RISC processor and DSP units for speech recognition. It includes GPIO pins for controlling external devices like relays and supports communication interfaces such as UART, I2C, and SPI.

This makes it suitable for offline voice-controlled home automation systems.
