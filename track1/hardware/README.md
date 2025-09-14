# Hardware / Embedded security

![rpi pinout](https://raw.githubusercontent.com/pinout-xyz/Pinout.xyz/master/resources/raspberry-pi-pinout.png "rpi pinout")

This is a very new domain, for all the club members. We recommend you get acquainted with basic electronics before starting these tasks, we shall assume you know what a breadboard is.

## How to get started

Try playing around with microcontrollers. For FPGAs, try [this](https://nandland.com/fpga-101/)

_If you're choosing this domain, then you don't have to solve any task in any other domains_
1. Task 0 - Simulate "hello world" on the [ESP32](https://wokwi.com/esp32)
2. Task 1 - 
    Solve *any one of these*
    1. Try this year's [qualification challenge for the CSAW ESC](https://github.com/TrustworthyComputing/csaw_esc_2025/tree/main/challenges/qualification). Final solution is not at all necessary, just an approach is enough
    2. Using an ESP32, write code that encrypts and decrypts some data, and perform power analysis. Can you tell when encryption and decryption happens? Try toggling GPIOs to measure timing differences. Even better if you can get your hands on an USB inline meter or an oscilloscope (RIG has one)
    3. Write a LED blinker for ESP32 with FreeRTOS. Use wokwi to simulate
3. Task 2 (Bonus) - Write a bootloader. for anything
