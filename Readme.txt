🚀 SCL Gaming Boost v1.3.0.0 🚀

-----

### 🎮 SCL Gaming Boost - Advanced Windows Optimization for Gamers 🎮

🔁 Summary of Improvements v1.3.0.0

🔁 Your Powershell script for the “SCL Gaming Boost” GUI has been improved with more robust functionality and a more robust code structure. The main changes include:

🔁 Improved Profile Logic: The FPS Boost and Streaming Mode profiles now have distinct behaviors. Streaming Mode explicitly keeps telemetry services and extra services active, which is essential for not interrupting background activities such as streaming software.

🔁 Button State Management: The script now correctly manages the state of the “Start/Stop Boost” button even when the Standard profile is selected while the boost is active.

🔁 Centralized Application Function: The Start-GamingBoost and Stop-GamingBoost functions have been replaced by a single Apply-BoostSettings function. This function manages the application of settings based on the selected profile and checkboxes, eliminating redundant logic in the button click event handler.

🔁 GUI Code Cleanup: The GUI code has been reorganized for better readability and a more structured flow.

🔁 Bug Fix: A bug has been fixed where the Standard profile did not correctly disable an already active boost.

🔁 I added a checkbox for “CPU Core Parking” and inserted the logic to activate the “Ultimate Performance” power plan.

🔁 New feature to detect and load the user's preferred language, adding a drop-down menu for language selection and dynamically updating the GUI text.

**SCL Gaming Boost** is a powerful Windows utility designed for demanding gamers. With a single click, it optimizes your operating system by disabling non-essential services, reducing telemetry, and applying intelligent tweaks to boost in-game performance.

**⚠️ Note:** Some optimizations require administrator rights. Be sure to run the program as an administrator.

-----

<img width="1800" height="927" alt="SCL Gaming Boost v1 3 0_v1 1" src="https://github.com/user-attachments/assets/9e795d90-996c-49d8-813d-00af29ae2f9e" />

<img width="1531" height="905" alt="SCL Gaming Boost v1 2 0_clean" src="https://github.com/user-attachments/assets/c0f40b01-422b-45ed-ada8-a35a2d3fa89c" />

* **https://vms.drweb-av.it/scan_file/**
-----

<img width="1800" height="1600" alt="Sniper Elite V2 Remastered Benchmark Performance Summary" src="https://github.com/user-attachments/assets/f7e076af-1f26-4e10-a5d2-04813c1eb253" />

-----


### 🚀 Key Features

  * **Customizable Boost Modes**: Activate targeted optimizations for gaming, streaming, or daily use.
      * **FPS Boost**: Maximizes performance in games.
      * **Streaming Mode**: Balances performance and stability for live streams.
      * **Standard**: Light optimizations for everyday use.
  * **Real-time Control**: View the active/inactive status directly from the GUI.
  * **Automatic Preference Saving**: The program remembers your last settings and Boost status.
  * **Quick System Restart**: A dedicated button to safely restart Windows.
  * **Detailed Operation Log**: All actions are recorded in a `.log` file for monitoring and debugging.
  * **Language Support**: Detects the user's preferred language and includes a drop-down menu for selection.

-----

### 🛠️ How to Use the Program

1.  **Download and Launch**: Go to the project's GitHub page and download the `SCL Gaming Boost.exe` file. Run it as an administrator (right-click → "Run as administrator").
2.  **Select Boost Mode**: In the GUI, choose the Boost mode that best suits your needs.
3.  **Apply Optimizations**: Press the **Boost** button. The program will disable services, modify the registry, and stop scheduled tasks. The optimization status will be visible in real time.
4.  **Restart System (Optional)**: After applying the Boost, you can click **Restart** to reboot your PC and ensure all changes take effect.

-----

### 🛡️ Optimizations Applied

  * **Services Disabled During Boost**:
      * `SysMain` (Superfetch)
      * `WSearch` (Indexing Service)
      * `DiagTrack` (Telemetry)
      * `Fax` (Fax Service)
      * `Spooler` (Print Spooler)
      * ...and other services not essential for gaming.
  * **Scheduled Tasks Disabled**:
      * `ProgramDataUpdater` (Application Experience)
      * `Proxy` (Autochk)
      * `Consolidator` (Customer Experience Improvement Program)
      * `UsbCeip` (USB Telemetry)
  * **Registry Changes**: Tweaks are applied to improve performance. All registry changes are **automatically reverted** when the Boost is disabled.

-----

### 📦 Distribution & Requirements

  * **Distribution**: The program is available as a single executable file for Windows. No installation is required.
  * **Requirements**:
      * Windows 10 or higher
      * PowerShell 5.0+
      * Administrative privileges

### 📜 License

This project is licensed under the **MIT License**. You are free to use, modify, and distribute it.

-----

**Developer**: [ilborga70](https://www.google.com/search?q=https://github.com/ilborga70) - Gamer, Developer, Serial Optimizer.
For contact and collaborations: [borgaccino@gmail.com](mailto:borgaccino@gmail.com)