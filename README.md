# README - Create Payload for Android with Meterpreter

## Description

This script automates the process of creating a payload for Android using Meterpreter and `msfvenom`. 
The generated payload allows establishing a reverse connection from an Android device to an attacking machine, facilitating penetration testing in controlled and legal environments.

## Requirements
- **Operating System**: Kali Linux or any system compatible with Metasploit.
- **Metasploit Framework**: Ensure that the Metasploit Framework is installed.
- **ADB Connection**: You will need ADB installed if you wish to transfer the APK to the Android device.

## Installation

**Step 1: Clone or download the script**
- Create a file named `create_payload.sh` and copy the provided script contents.

**Step 2: Grant execution permissions**
- chmod +x create_payload.sh

**Step 3: Ensure Metasploit is installed**
- sudo apt update
- sudo apt install -y metasploit-framework

## Usage

**Step 1: Edit the script**
- Open `create_payload.sh` and replace `<your_ip>` with your attacker's IP address.
- Replace `<port>` with the desired port (e.g., 4444).

**Step 2: Run the script**
./create_payload.sh

**Step 3: Transfer the APK**
- Use ADB or any other method to transfer `payload.apk` to the Android device.
- Ensure that the device has installations from unknown sources enabled.

**Step 4: Start the listener in Metasploit**
- The script already configures and starts the listener automatically.

**Step 5: Capture the session**
- When the user opens the APK on the Android device, you should see an active Meterpreter session in your Metasploit terminal.

## Important Notes
- **Ethics and Legality**: This script is for educational purposes only. Ensure you have the appropriate consent before conducting penetration tests. Creating and running payloads without authorization is illegal and unethical.
- **Security**: Keep the environment secure and do not use this script on devices or networks without permission.

## Contributions
If you would like to contribute to improving this script or adding new functionalities, feel free to send a pull request or open an issue.

## License
This project is licensed under the MIT License. See the LICENSE file for more details.
