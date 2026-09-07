---
title: NRF24L01+ Transmitter/Receiver
date: 2026-08-27 16:58:00 -500
categories: [STM32, RF]
tags: [electronics, stm32, rf]
image:
  path: /assets/img/nrf24l01/stm32l432kc-nrf24l01-joysticks.jpg
  alt: 1/24 Bronco wired up to the STM32, DRV8874 and battery.
---

## About
The NRF24L01 is an awesome little radio transceiver IC from Nordic. It operates at 2.4Ghz, has a range of about 100 meters (at least with the modules/antennas used in this demo) and can be controlled using the SPI protocol.

For this demo, I’ve set up two STM32 Nucleo boards to control a pair of NRF24L01 modules. The first STM32 sets its NRF as a transmitter and takes input from two joysticks. It then packages up the joystick data and sends it over the air to the other NRF/STM32 pair. The receiver STM32 then logs the joystick axes to the console.

## Components
- 2x STM32 Nucleo L432KC
- 2x NRF24L01+ Modules
- 2x joysticks
