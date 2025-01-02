<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>README - Cardputer Setup</title>
</head>
<body>
    <h1>Cardputer Setup Guide</h1>

    <h2>Requirements</h2>
    <ul>
        <li>M5 Cardputer</li>
        <li>SD Card</li>
    </ul>

    <h2>1. Installation</h2>

    <h3>1.1 Preparing the SD Card</h3>
    <p>Format the SD card to FAT32.</p>

    <h3>1.2 Installing M5 Burner</h3>
    <ol>
        <li>Visit the <a href="https://www.m5stack.com">M5Stack website</a>.</li>
        <li>Navigate to the Software section and download the M5 Burner ZIP file.</li>
        <li>Extract the ZIP and run <code>M5Burner.exe</code>. Update the software if prompted.</li>
    </ol>

    <img src=\"assets/Imagens/1.2.png\" alt=\"M5 Burner Installation\" />

    <h3>1.3 Installing M5Launcher</h3>
    <ol>
        <li>In M5 Burner, select the <strong>CARDPUTER</strong> tab.</li>
        <li>Locate and download the <code>M5Launcher.bin</code> firmware.</li>
        <li>Connect the Cardputer to your computer and click <strong>Burn</strong>.</li>
        <li>Select the appropriate COM port and click <strong>Start</strong>. Avoid disconnecting during the flashing process.</li>
    </ol>
    <p>Once successfully installed, the firmware will be ready to use.</p>

    <img src=\"assets/Imagens/1.3.png\" alt=\"Burning Firmware\" />

    <h3>1.4 Configuring M5Launcher</h3>

    <h4>1.4.1 SD Card Verification</h4>
    <p>Ensure the SD option is accessible on the home screen. A green icon indicates readiness, while a gray icon indicates issues.</p>

    <img src=\"assets/Imagens/1.4.1.png\" alt=\"SD Card Verification\" />

    <h4>1.4.2 Activating Web Interface</h4>
    <p>Select the <strong>WUI</strong> icon to configure the web interface in one of the following modes:</p>
    <ul>
        <li><strong>My Network:</strong> Connect to an existing Wi-Fi network by providing credentials.</li>
        <li><strong>AP Mode:</strong> Start an open Wi-Fi network hosted by the Cardputer.</li>
    </ul>

    <p>After selecting a mode, the Cardputer will display an IP address for browser access. Use the provided login credentials to access the web interface.</p>
    <p>The interface allows file management, storage monitoring, and firmware version checks.</p>

    <img src=\"assets/Imagens/1.4.2.png\" alt=\"Web Interface Setup\" />

    <h4>1.4.3 Downloading Secondary Firmwares</h4>
    <p>To enable multi-boot, add necessary firmware binaries:</p>
    <ol>
        <li>Visit the GitHub repository of <code>Evil-Cardputer</code>: <a href="https://github.com/7h30th3r0n3/Evil-M5Core2/tree/main/binaries">Evil M5Core2 Binaries</a>.</li>
        <li>Alternatively, download the firmware via the web interface under <strong>Online Firmware List</strong>.</li>
        <li>Upload the <code>.bin</code> file to the Cardputer via the web interface.</li>
    </ol>

    <h3>1.5 Installing Evil-Cardputer</h3>
    <ol>
        <li>Disable the web interface by clicking <strong>OK</strong>.</li>
        <li>From the home menu, select <strong>SD</strong> and locate the uploaded <code>.bin</code>.</li>
        <li>Choose <strong>Install</strong> and wait for the process to complete. The device will restart automatically.</li>
    </ol>

    <img src=\"assets/Imagens/1.5.png\" alt=\"Installing Evil-Cardputer\" />

    <p>Your Cardputer is now configured and ready for use!</p>
</body>
</html>
