# The Smallest DIY Spy Cam

Welcome to the repository for **The Smallest DIY Spy Cam** project. This project features a compact, easy-to-build camera using the Xiao ESP32S3 Sense, capable of capturing and saving images to an SD card with just the press of a button. It's perfect for DIY enthusiasts who love working on mini electronics projects.

## Features

- **Small and Discreet**: Built using the Xiao ESP32S3 Sense, making it one of the smallest DIY cameras available.
- **Image Capture**: Captures images with a simple button press.
- **Sequential Image Naming**: Images are automatically named in sequence (image1, image2, image3, etc.).
- **SD Card Storage**: Images are stored directly on an SD card.
- **Power-Saving Mode**: A long press of the button puts the device into deep sleep, where it consumes minimal power. It wakes up and turns on the LED when a long press is detected again.


## Components Used

- Xiao ESP32S3 Sense (With camera) 
- Micro SD Card Module
- Push Buttons (for capturing images)
- LiPo Battery
- Wires
- RGB LED


## Setup Instructions

1. **Hardware Assembly**
   - Connect the camera module to the Xiao ESP32S3 Sense.
   - Connect the SD card module.
   - Wire the capture button to pin D0 and the other pin on the GND pin.
   - Solder the battery for portable power.

2. **Software**
   - Clone this repository to your local machine.
   - Open the project VSCode and install the PlatformIO Plugin.
   - Select the Xiao ESP32S3 board.
   - Upload the code to the board.
  
 **Guide to Selecting the Right Code**
   This repository contains two versions of the project. Depending on your requirements, you can choose between the Basic Image Capture version or the Image Capture with Power-Saving (Deep Sleep) version:

   **Basic Image Capture:**

   Use this code if: You want a straightforward implementation where pressing the button captures an image and saves it to the SD card. This version does not include any power-saving features and is ideal for short-term use or situations where power consumption is not a    concern.
   Ideal for: Quick projects, demonstrations, or when you have a continuous power supply.
   File Name: 'code.ino'

   **Image Capture with Power-Saving (Deep Sleep):**

   Use this code if: You need your camera to operate for extended periods without draining the battery. This version allows you to put the device into deep sleep with a long press of the button and wake it up again with another long press. It also includes the basic          image capture functionality with a short press.
   Ideal for: Remote deployments, battery-powered applications, or scenarios where energy efficiency is crucial.
   File Name: 'DeepSleep.ino'



4. **Operation**
   - Power on the camera by pressing the button once.
   - Press the  button to take a picture.
   - The image will be saved to the SD card with a sequential name.
   - To turn of the camera, just long press the button for 2 seconds

## Usage

 - TinyML Image Data Collection: This spy camera is ideal for collecting image datasets in remote areas for machine learning projects. The power-saving mode extends battery life, making it more suitable for fieldwork.
 - DIY Spy Camera: The small form factor, along with the ability to operate in low-power mode, makes it a great tool for DIY enthusiasts interested in creating their own spy or security cameras.

## Future Enhancements

- Adding video recording functionality.
- Implementing wireless image transfer.

## License

This project is licensed under the MIT License. See the LICENSE file for details.

## Acknowledgments

- Special thanks to the open-source community for their contributions and support.

