# Pomodoro Timer for ESP32-C6

A Pomodoro timer application designed for the Waveshare ESP32-C6 with 1.47 inch display.

## Overview

This project implements a Pomodoro Technique timer on the ESP32-C6 microcontroller, utilizing the Waveshare 1.47 inch display for visual feedback. The Pomodoro Technique is a time management method that uses a timer to break work into intervals, traditionally 25 minutes in length, separated by short breaks.

## Hardware Requirements

- **Microcontroller**: Waveshare ESP32-C6
- **Display**: Waveshare 1.47 inch display
- **Additional components**: (to be documented)

## Features

- (Features to be added as development progresses)

## Getting Started

### Prerequisites

- Arduino IDE or PlatformIO
- ESP32 board support package
- Waveshare display library

### Installation

1. Clone this repository:
   ```bash
   git clone <repository-url>
   cd pomidoro
   ```

2. Install required libraries:

   **Using PlatformIO (Recommended):**
   ```bash
   # Libraries are automatically installed when building
   pio run
   ```
   
   **Using Arduino IDE:**
   - Open Arduino IDE
   - Go to Sketch > Include Library > Manage Libraries
   - Install the following libraries:
     - TFT_eSPI (by Bodmer) - Version 2.5.43+
     - LVGL (Light and Versatile Graphics Library) - Version 9.0.0+
     - FastLED - Version 3.6.0+
     - Adafruit GFX Library - Version 1.11.9+
     - Adafruit BusIO - Version 1.14.5+
   
   See `libraries.txt` for detailed library information.

3. Configure your development environment:
   
   **PlatformIO:**
   - The `platformio.ini` file is already configured
   - Select the `esp32-c6-devkitc-1` environment
   
   **Arduino IDE:**
   - Install ESP32 board support: https://docs.espressif.com/projects/arduino-esp32/en/latest/installing.html
   - Select Board: ESP32C6 Dev Module
   - Configure TFT_eSPI library's `User_Setup.h` for your display

### Building and Uploading

**PlatformIO:**
```bash
# Build the project
pio run

# Upload to device
pio run --target upload

# Monitor serial output
pio device monitor
```

**Arduino IDE:**
- Click the Upload button
- Monitor via Tools > Serial Monitor (115200 baud)

## Usage

- (Usage instructions to be added)

## Required Libraries

- **TFT_eSPI** - Display driver for ST7789 (1.47 inch display)
- **LVGL** - Advanced GUI library (optional)
- **FastLED** - RGB LED control
- **Adafruit GFX Library** - Graphics primitives
- **Adafruit BusIO** - I2C/SPI communication

See `libraries.txt` for detailed library information and installation instructions.

## Project Structure

```
pomidoro/
├── platformio.ini          # PlatformIO configuration with library dependencies
├── pomidoro_esp32-C6/      # Main project directory
│   ├── LICENSE            # MIT License
│   ├── libraries.txt      # Detailed library documentation
│   └── README.md          # This file
└── .gitignore             # Git ignore rules
```

## License

This project is licensed under the MIT License - see the [LICENSE](pomidoro_esp32-C6/LICENSE) file for details.

## Contributing

- (Contributing guidelines to be added)

## Author

HaroldSP

## Acknowledgments

- (Acknowledgments to be added)

