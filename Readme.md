# Enigma2 Roku Streaming Channel

This Roku channel allows users to stream content from Enigma2-based satellite receivers.

## Table of Contents

- [Features](#features)
- [Requirements](#requirements)
- [Setup](#setup)
- [Development Guide](#development-guide)
- [Scenes Description](#scenes-description)
- [Folder Structure](#folder-structure)
- [Deployment](#deployment)
- [FAQ](#faq)
- [License](#license)
- [Support](#support)

## Features

1. **Display Enigma2 Channel List:**
Upon launching the application, the channel list is automatically retrieved from the Enigma2 box and presented to the users. They can scroll through the list and select a channel. If the TV channels on the Enigma2 box have a logo (picon), it will also be displayed in the Enigma2 Channel List.

2. **Stream Channel:**
After selecting a channel, users can initiate streaming by clicking on it. The application automatically fetches the M3U8 file for the selected channel and starts streaming.

3. **Adjust Settings:**
Users can access the settings to configure the connection information to their Enigma2 box. Here, they can set up the hostname, web interface port, streaming port, username, password, and other options. The application supports authentication for accessing the Enigma2 box if required. Users can provide their credentials in the settings. Users also have the option to choose between using a secure HTTPS connection or the default HTTP connection for accessing the Enigma2 box.

## Requirements

Please note that the Enigma2 Streaming Channel is currently not available in the official Roku Store. It can only be installed on Roku devices that are in developer mode. To run this project and deploy it on a Roku device, you'll need the following:

- A Roku device in developer mode
- Node.js and npm
- Visual Studio Code (or any other IDE of your choice)

## Setup

1. Ensure your Roku device is in developer mode. See the [Roku Developer Guide](https://developer.roku.com/en-gb/docs/developer-program/getting-started/developer-setup.md) for instructions.
2. Clone this repository to your local machine:

   ```bash
   git clone https://github.com/madoe21/Enigma2-Roku-Streaming-Channel.git
   ```

3. Navigate to the project directory:

   ```bash
   cd Enigma2RokuStreamingChannel
   ```

4. Install the dependencies:

   ```bash
   npm install
   ```

## Development Guide

1. Open the project in Visual Studio Code:

   ```bash
   code .
   ```

2. Edit the files in `source/` according to your requirements.

3. Build the application:

   ```bash
   npm run build
   ```

## Scenes Description

For a detailed description of each scene, please refer to [Scenes.md](Scenes.md).

## Folder Structure

For detailed information about the folder structure of the project, please refer to [Structure.md](Structure.md).

```
Enigma2RokuStreamingChannel/
├── source/ 
│   ├── components/
│   ├── fonts/
│   ├── images/
│   ├── locale/
│   ├── source/
│   └── manifest
├── bsconfig.json
├── package.json
└── README.md
```

## Deployment

Run one of the following scripts to deploy the application to your Roku device:

   - `npm run build`: Builds the application - no deployment possible.
   - `npm run package`: Packages the application - manual deployment possible.
   - `npm run deploy`: Deploys the application to the Roku device automatically (according to `bsconfig.json`).

## FAQ

### What is Enigma2?
Enigma2 is an open-source software based on Linux used in satellite and cable receivers. It provides a user-friendly interface for watching television programs, recording shows, streaming media, and more. Enigma2 is utilized by various manufacturers such as Dreambox, Gigablue, AzBox, VU+, and Xtrend in their receivers.

### What is Roku?
Roku is a brand of digital media players developed and distributed by Roku, Inc. These devices allow users to access a variety of streaming services and channels on their televisions. Roku players offer a user-friendly interface and support a wide range of apps for streaming, music, games, and more.

### What Roku devices are available for streaming?
Roku offers a variety of devices, including:

- **Roku Streaming Stick:**
A compact HDMI stick that plugs directly into the HDMI port of the television, providing an easy plug-and-play solution.
- **Roku Express:**
An affordable streaming device that offers a great streaming experience at an affordable price.
- **Roku Ultra:**
Roku's premium streaming device that offers advanced features such as 4K and HDR streaming, enhanced Wi-Fi performance, and an expanded feature set.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Support
I appreciate everyone who supports me and the project! For any requests and suggestions, feel free to provide feedback.

[![Buy Me A Coffee](https://cdn.buymeacoffee.com/buttons/default-orange.png)](https://www.buymeacoffee.com/madoe21)
