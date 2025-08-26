# 🎮 SCL Gaming Boost v1.6.0 — Benchmark & Features

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
  - 🎯 FPS Boost
  - 📺 Streaming Mode
  - 🧩 Standard Mode
- **Real-time Control Panel**
- **Automatic Preference Saving**
- **Quick System Restart**
- **Detailed Operation Log**
- **Multi-language Support**

---

## 🛡️ Optimizations Applied

### 🔧 Services Disabled

- `SysMain` (Superfetch)  
- `WSearch` (Indexing Service)  
- `DiagTrack` (Telemetry)  
- `Fax`  
- `Spooler`  
- `Disable hibernation`  
- `Disable mouse acceleration`  
- `Optimize Windows Update services`  

### 📅 Scheduled Tasks Disabled

- `ProgramDataUpdater`  
- `Proxy`  
- `Consolidator`  
- `UsbCeip`  

### 🧬 Registry Tweaks

| Registry Key | Value Set | Description |
|--------------|-----------|-------------|
| `HKLM\SOFTWARE\Policies\Microsoft\Windows\DataCollection` | `AllowTelemetry: 0` | Disables telemetry |
| `HKLM\SYSTEM\CurrentControlSet\Control\PriorityControl` | `Win32PrioritySeparation: 26` | Optimizes thread priority |
| `HKCU\Software\Microsoft\Windows\CurrentVersion\Explorer\VisualEffects` | `VisualFXSetting: 2` | Disables visual effects |
| `HKCU\SOFTWARE\Microsoft\Windows\CurrentVersion\GameDVR` | `AppCaptureEnabled: 0` | Disables game recording |
| `HKCU\SOFTWARE\Microsoft\GameBar` | `ShowStartupPanel: 0` | Hides Game Bar |
| `HKCU\SOFTWARE\Microsoft\GameBar` | `AutoGameModeEnabled: 0` | Disables auto Game Mode |
| `HKCU\SOFTWARE\Microsoft\GameBar` | `AllowAutoGameMode: 1` | Enables manual Game Mode |
| `HKLM\SYSTEM\CurrentControlSet\Control\Session Manager\Memory Management` | `LargeSystemCache: 1` | Optimizes system cache |
| `HKLM\SYSTEM\CurrentControlSet\Control\Session Manager\Memory Management` | `DisablePagingExecutive: 1` | Keeps drivers in RAM |

---

## 🚀 NEW OPTIMIZATIONS FOR AN EXTRA BOOST

- 🔕 **Disable Windows Notifications**: Prevents micro-stuttering and distractions during gameplay.
- 🧠 **Set Game Process Priority**: Ensures the game gets maximum CPU allocation.
- 🌐 **Disable Network Card Power Saving**: Prevents bandwidth throttling and latency spikes.
- 🧹 **Clear DNS Cache**: Resolves connection issues and improves response times.
- 💾 **Disable Hibernation**: Frees up disk space and reduces system load.
- 🎯 **Disable Mouse Acceleration**: Improves pointer accuracy.
- 🔄 **Optimize Windows Update Services**: Prevents background resource usage.

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