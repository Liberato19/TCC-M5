# Cardputer Setup Guide

## Requirements
- M5 Cardputer
- SD Card

## 1. Installation

### 1.1 Preparing the SD Card
Format the SD card to FAT32.

### 1.2 Installing M5 Burner
1. Visit the [M5Stack website](https://www.m5stack.com).
2. Navigate to the Software section and download the M5 Burner ZIP file.
3. Extract the ZIP and run `M5Burner.exe`. Update the software if prompted.

![M5 Burner Installation](assets/Imagens/1.2.png)

### 1.3 Installing M5Launcher
1. In M5 Burner, select the **CARDPUTER** tab.
2. Locate and download the `M5Launcher.bin` firmware.
3. Connect the Cardputer to your computer and click **Burn**.
4. Select the appropriate COM port and click **Start**. Avoid disconnecting during the flashing process.

Once successfully installed, the firmware will be ready to use.

![Burning Firmware](assets/Imagens/1.3.png)

### 1.4 Configuring M5Launcher

#### 1.4.1 SD Card Verification
Ensure the SD option is accessible on the home screen. A green icon indicates readiness, while a gray icon indicates issues.

![SD Card Verification](assets/Imagens/1.4.1.png)

#### 1.4.2 Activating Web Interface
Select the **WUI** icon to configure the web interface in one of the following modes:
- **My Network:** Connect to an existing Wi-Fi network by providing credentials.
- **AP Mode:** Start an open Wi-Fi network hosted by the Cardputer.

After selecting a mode, the Cardputer will display an IP address for browser access. Use the provided login credentials to access the web interface.

The interface allows file management, storage monitoring, and firmware version checks.

![Web Interface Setup](assets/Imagens/1.4.2.png)

#### 1.4.3 Downloading Secondary Firmwares
To enable multi-boot, add necessary firmware binaries:
1. Visit the GitHub repository of `Evil-Cardputer`: [Evil M5Core2 Binaries](https://github.com/7h30th3r0n3/Evil-M5Core2/tree/main/binaries).
2. Alternatively, download the firmware via the web interface under **Online Firmware List**.
3. Upload the `.bin` file to the Cardputer via the web interface.

### 1.5 Installing Evil-Cardputer
1. Disable the web interface by clicking **OK**.
2. From the home menu, select **SD** and locate the uploaded `.bin`.
3. Choose **Install** and wait for the process to complete. The device will restart automatically.

![Installing Evil-Cardputer](assets/Imagens/1.5.png)

Your Cardputer is now configured and ready for use!
