# SCL Gaming Boost v1.9.0.0

<img width="1913" height="1094" alt="SCL Gaming Boost v1 9 0 0" src="https://github.com/user-attachments/assets/f8d96da5-8697-4153-8e0b-99a755c748a7" />

**Disclaimer**: You can check suspicious files for malicious programs free of charge using the Dr.Web online file scanner: https://vms.drweb-av.it/scan_file/

---

## 🧪 Benchmark: Sniper Elite V2 Remastered
**Windows 11 Game Mode vs. SCL Gaming Boost**

We ran two benchmark tests using identical hardware and graphics settings. The only difference? One test used Windows 11's built-in Game Mode, while the other added **SCL Gaming Boost**.

### 🖥️ Test Setup

- **CPU**: Intel Core i5-13600KF
- **GPU**: NVIDIA GeForce RTX 4080
- **RAM**: 64 GB
- **Resolution**: 2560 x 1080
- **Graphics Settings**: ULTRA preset, V-Sync OFF, Supersampling OFF

---

### 📊 Performance Comparison

| Metric | Game Mode Only | Game Mode + SCL Gaming Boost |
|----------------------|----------------|-------------------------------|
| **Average FPS** | 710.9 | 730.3 |
| **Minimum FPS** | 226.4 | 270.2 |
| **Maximum FPS** | 1378.4 | 1342.3 |
| **Avg. Frame Time** | 1.407 ms | 1.369 ms |
| **Min. Frame Time** | 0.725 ms | 0.745 ms |
| **Max. Frame Time** | 4.416 ms | 3.700 ms |

---

### 🧠 Analysis & Takeaways

- ✅ **+2.7% Average FPS** boost
- 🚀 **+19.3% Minimum FPS** improvement
- ⚡ **Lower Average Frame Time** = snappier responsiveness
- 📉 Slight dip in Max FPS is negligible
- 🧩 **Reduced Max Frame Time** = smoother pacing

---

## 🏁 Final Verdict

**SCL Gaming Boost** delivers measurable performance gains, especially in minimum FPS and frame time consistency. Ideal for competitive or high-refresh gaming.

---

## ⚙️ What Is SCL Gaming Boost?

A lightweight Windows utility that disables non-essential services, reduces telemetry, and applies intelligent tweaks to boost in-game performance.

> ⚠️ Some optimizations require administrator rights. Run the program as an administrator.

---

## 🎮 Key Features

- **Customizable Boost Modes**:
    - 🎯 **FPS Boost**: Maximizes frame rate by disabling non-critical services.
    - 📺 **Streaming Mode**: Optimizes for streaming by keeping essential services active.
    - 🧩 **Standard Mode**: Safely restores your system to its original state by using a **backup of your personal settings**, not just default values.
- **Real-time Control Panel**
- **Automatic Preference Saving**
- **Quick System Restart**
- **Detailed Operation Log**
- **Multi-language Support**

---

### 🔧 Services Disabled

- `SysMain` (Superfetch)
- `WSearch` (Indexing Service)
- `DiagTrack` (Telemetry)
- `Fax`
- `Spooler`
- `WMPNetworkSvc` (Windows Media Player Network Sharing Service)
- `XblGameSave` (Xbox Game Save)
- `BluetoothSupportService`
- `RemoteRegistry`
- `PhoneSvc`

### 📅 Scheduled Tasks Disabled

- `ProgramDataUpdater`
- `Proxy`
- `Consolidator`
- `UsbCeip`

### 🧬 Registry Tweaks

| Registry Key | Value Set | Description |
|---|---|---|
| `HKLM\SOFTWARE\Policies\Microsoft\Windows\DataCollection` | `AllowTelemetry: 0` | Disables telemetry. |
| `HKLM\SYSTEM\CurrentControlSet\Control\PriorityControl` | `Win32PrioritySeparation: 26` | Optimizes thread priority for games. |
| `HKCU\Software\Microsoft\Windows\CurrentVersion\Explorer\VisualEffects` | `VisualFXSetting: 2` | Disables visual effects. |
| `HKCU\SOFTWARE\Microsoft\Windows\CurrentVersion\GameDVR` | `AppCaptureEnabled: 0` | Disables game recording. |
| `HKCU\SOFTWARE\Microsoft\GameBar` | `ShowStartupPanel: 0` | Hides Game Bar. |
| `HKCU\SOFTWARE\Microsoft\GameBar` | `AutoGameModeEnabled: 0` | Disables auto Game Mode. |
| `HKCU\SOFTWARE\Microsoft\GameBar` | `AllowAutoGameMode: 1` | Enables manual Game Mode. |
| `HKLM\SYSTEM\CurrentControlSet\Control\Session Manager\Memory Management` | `LargeSystemCache: 1` | Optimizes system cache. |
| `HKLM\SYSTEM\CurrentControlSet\Control\Session Manager\Memory Management` | `DisablePagingExecutive: 1` | Keeps drivers in RAM. |

---

### ✨ New Optimizations for an Extra Boost

This version introduces a series of new powerful optimizations to take your performance to the next level. Each option can be enabled or disabled via the convenient user interface.

| Optimization | Detailed Description |
|---|---|
| 🔕 **Disable Windows Notifications** | Disables system notifications to prevent annoying pop-ups and micro-stuttering that can disrupt gaming fluidity. |
| 🧠 **Set Game Process Priority** | Ensures your game receives maximum CPU resource allocation. The script identifies the foreground process and sets its priority to "High" to ensure it always has precedence. |
| 🌐 **Disable Network Card Power Saving** | Prevents the system from throttling your network card's bandwidth. This optimization is crucial for preventing lag and latency spikes during online gaming sessions. |
| 🧹 **Clear DNS Cache** | Clears the system's DNS cache to resolve potential connection issues and improve response times (ping) with gaming servers. |
| 💾 **Disable Hibernation** | Disables the hibernation feature to free up valuable disk space (the `hiberfil.sys` file) and reduce overall system load. |
| 🎯 **Disable Mouse Acceleration** | Removes mouse pointer acceleration at the operating system level. This provides greater precision and a 1:1 response, essential for FPS games and e-sports. |
| 🔄 **Optimize Windows Update Services** | Prevents Windows Update from downloading and installing updates in the background while you're gaming, reducing resource usage and preventing FPS drops. |

---

## ⚙️ How It Works

The tool temporarily modifies the following system settings to maximize performance:

* **Disable Telemetry and Unnecessary Services**: Stops background services and telemetry activities that consume CPU and network cycles.
* **CPU Management**: Disables CPU "Core Parking" and activates the "Ultimate Performance" power plan to ensure the processor runs at its full capacity.
* **System Optimizations**: Applies registry modifications to optimize memory management, visual interface effects, and other basic settings.
* **Xbox Services Management**: Disables services related to the Game Bar and the Xbox app that can impact performance.
* **Network & I/O**: Tweaks network settings to reduce latency and improves I/O performance by managing the system cache.

## ⚠️ Warning

* **Run as Administrator**: This script must be run with administrator permissions to apply modifications to the system registry and services.
* **Compatibility**: Designed for Windows 10 and 11. It may not work correctly on earlier versions of Windows.
* **Safe Restore**: The "Standard" mode now restores your PC to its **original state** by using a backup file, ensuring a safe and reversible process.

---

## 🛠️ How to Use

1. **Download** the `.exe` from GitHub
2. **Run as Administrator**
3. **Select Boost Mode**
4. **Click Boost**
5. **(Optional)** Restart your system

---

## 📦 Distribution & Requirements

- **Type**: Portable `.exe` (No installation required)
- **OS**: Windows 10 or higher
- **PowerShell**: 5.0+
- **Permissions**: Admin rights required

---

## 📜 License

Licensed under the **MIT License** — free to use, modify, and distribute.

---

## 👤 Developer

**ilborga70** — Gamer, Developer, Serial Optimizer
📧 [borgaccino@gmail.com](mailto:borgaccino@gmail.com)

🔗 [GitHub Profile](https://github.com/ilborga70)
