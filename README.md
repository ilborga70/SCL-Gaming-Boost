# 🚀 SCL Gaming Boost v1.4.0.0 🚀

<img width="1913" height="1220" alt="SCL Gaming Boost v1 4 0" src="https://github.com/user-attachments/assets/f3f3f932-deff-480b-801f-f507a78c9674" />

**Disclaimer**: You can check suspicious files for malicious programs free of charge using the Dr.Web online file scanner: [https://vms.drweb-av.it/scan\_file/](https://vms.drweb-av.it/scan_file/)


-----

**SCL Gaming Boost** is a powerful Windows utility designed for demanding gamers. With a single click, it optimizes your operating system by disabling non-essential services, reducing telemetry, and applying intelligent tweaks to boost in-game performance.

**⚠️ Note:** Some optimizations require administrator rights. Be sure to run the program as an administrator.

-----

## 🎮 Key Features

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

## 🛡️ Optimizations Applied

### Services Disabled During Boost

  * `SysMain` (Superfetch)
  * `WSearch` (Indexing Service)
  * `DiagTrack` (Telemetry)
  * `Fax` (Fax Service)
  * `Spooler` (Print Spooler)
  * `Disable hibernation` (Frees up disk space and reduces system load)
  * `Disable mouse acceleration` (Improves pointer accuracy in games)
  * `Optimize Windows Update services` (Prevents bandwidth usage and resource consumption in the background)
  * ...and other services not essential for gaming.

### Scheduled Tasks Disabled

  * `ProgramDataUpdater` (Application Experience)
  * `Proxy` (Autochk)
  * `Consolidator` (Customer Experience Improvement Program)
  * `UsbCeip` (USB Telemetry)

### Registry Changes

Tweaks are applied to improve performance. All registry changes are **automatically reverted** when the Boost is disabled.

| Registry Key                                                             | Value Set | Description                                                       |
| ------------------------------------------------------------------------ | --------- | ----------------------------------------------------------------- |
| `HKLM\SOFTWARE\Policies\Microsoft\Windows\DataCollection`                | `AllowTelemetry: 0` | Disables telemetry                                                |
| `HKLM\SYSTEM\CurrentControlSet\Control\PriorityControl`                  | `Win32PrioritySeparation: 26` | Optimizes thread priority                                         |
| `HKCU\Software\Microsoft\Windows\CurrentVersion\Explorer\VisualEffects`  | `VisualFXSetting: 2` | Disables visual effects                                           |
| `HKCU\SOFTWARE\Microsoft\Windows\CurrentVersion\GameDVR`                 | `AppCaptureEnabled: 0` | Disables automatic game recording                                 |
| `HKCU\SOFTWARE\Microsoft\GameBar`                                        | `ShowStartupPanel: 0` | Hides Game Bar panel on startup                                   |
| `HKCU\SOFTWARE\Microsoft\GameBar`                                        | `AutoGameModeEnabled: 0` | Disables automatic Game Mode                                      |
| `HKCU\SOFTWARE\Microsoft\GameBar`                                        | `AllowAutoGameMode: 1` | Allows manual Game Mode                                           |
| `HKLM\SYSTEM\CurrentControlSet\Control\Session Manager\Memory Management` | `LargeSystemCache: 1` | Optimizes system cache                                            |
| `HKLM\SYSTEM\CurrentControlSet\Control\Session Manager\Memory Management` | `DisablePagingExecutive: 1` | Keeps drivers in RAM for better performance                       |

-----

## 🛠️ How to Use the Program

1.  **Download and Launch**: Go to the project's GitHub page and download the `SCL Gaming Boost.exe` file. Run it as an administrator (right-click → "Run as administrator").
2.  **Select Boost Mode**: In the GUI, choose the Boost mode that best suits your needs.
3.  **Apply Optimizations**: Press the **Boost** button. The program will disable services, modify the registry, and stop scheduled tasks. The optimization status will be visible in real time.
4.  **Restart System (Optional)**: After applying the Boost, you can click **Restart** to reboot your PC and ensure all changes take effect.

-----

## 📦 Distribution & Requirements

  * **Distribution**: The program is available as a single executable file for Windows. No installation is required.
  * **Requirements**:
      * Windows 10 or higher
      * PowerShell 5.0+
      * Administrative privileges

-----

## 📜 License

This project is licensed under the **MIT License**. You are free to use, modify, and distribute it.

-----

**Developer**: [ilborga70](https://www.google.com/search?q=https://github.com/ilborga70) - Gamer, Developer, Serial Optimizer.
For contact and collaborations: [borgaccino@gmail.com](mailto:borgaccino@gmail.com)


