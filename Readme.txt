
<img width="1913" height="1220" alt="SCL Gaming Boost v1 4 0" src="https://github.com/user-attachments/assets/f3f3f932-deff-480b-801f-f507a78c9674" />

**Disclaimer**: You can check suspicious files for malicious programs free of charge using the Dr.Web online file scanner: [https://vms.drweb-av.it/scan\_file/](https://vms.drweb-av.it/scan_file/)

---

## 🎮 Sniper Elite V2 Remastered Benchmark: Windows 11 Game Mode vs. SCL Gaming Boost

We ran two benchmark tests on Sniper Elite V2 Remastered using identical hardware and graphics settings. The only difference? One test used Windows 11's built-in Game Mode, while the other added a feature called **SCL Gaming Boost**.

### 🖥️ Test Setup (Identical for Both Runs)

- **CPU:** Intel Core i5-13600KF  
- **GPU:** NVIDIA GeForce RTX 4080  
- **RAM:** 64 GB  
- **Resolution:** 2560 x 1080  
- **Graphics Settings:** ULTRA preset, V-Sync OFF, Supersampling OFF  

---

### 📊 Performance Comparison

| Metric                | Game Mode Only | Game Mode + SCL Gaming Boost |
|----------------------|----------------|-------------------------------|
| **Average FPS**      | 710.9          | 730.3                         |
| **Minimum FPS**      | 226.4          | 270.2                         |
| **Maximum FPS**      | 1378.4         | 1342.3                        |
| **Avg. Frame Time**  | 1.407 ms       | 1.369 ms                      |
| **Min. Frame Time**  | 0.725 ms       | 0.745 ms                      |
| **Max. Frame Time**  | 4.416 ms       | 3.700 ms                      |

---

### 🧠 Analysis & Takeaways

The clear winner here is the setup with **SCL Gaming Boost** enabled. Here's why:

- ✅ **Average FPS** increased by ~2.7%, from 710.9 to 730.3. That means smoother overall performance and more frames rendered per second.
- 🚀 **Minimum FPS** jumped from 226.4 to 270.2 — a crucial improvement for gameplay fluidity. Higher minimums reduce sudden frame drops and micro-stutters.
- ⚡ **Average Frame Time** dropped from 1.407 ms to 1.369 ms. Lower frame times = faster image rendering = snappier responsiveness.
- 📉 **Maximum FPS** dipped slightly (1378.4 → 1342.3), but this has negligible impact since both values far exceed the 200 Hz refresh rate of the monitor.
- 🧩 **Maximum Frame Time** saw a notable reduction (4.416 ms → 3.700 ms), meaning fewer extreme spikes and smoother frame pacing.

---

### 🏁 Final Verdict

If you're chasing ultra-smooth gameplay and stability, enabling **SCL Gaming Boost** on top of Windows 11 Game Mode delivers measurable benefits — especially in minimum FPS and frame time consistency. It's not a massive leap, but it's a meaningful one for competitive or high-refresh gaming.

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