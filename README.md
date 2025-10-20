## 🎮 SCL Gaming Boost v3.5.1 + PC Performance Test Pro 2025🎮�

## ![🎮 SCL Gaming Boost v3 5 0 + PC Performance Test Pro 2025🎮](https://github.com/user-attachments/assets/bdf90b97-c991-4916-8e0c-5a90e6ad6577)

## 🔧 Migliorie e Funzionalità Principali

1. 🌍 Aggiornamento Online: Creata funzione Update-DatabaseFromOnline che punta correttamente al nuovo Gist e usa Normalize-BenchmarkToScore.

2. 🗃️ Auto-apprendimento: Aggiunto funzioni Update-DatabaseWithDetectedComponents e Save-DatabaseAfterScan.
In questo modo, il database locale "impara" i componenti che non conosce utilizzando i punteggi di fallback, per poi salvarli.

3. 🌐 Localizzazione: Ampliato enormemente il dizionario $DICT.

1. 🗃️ Database e Valutazione Avanzata
Punteggi Precisi: Utilizza un Sistema di Database Dinamico (locale e aggiornabile online) con punteggi basati su benchmark reali (es. PassMark) per CPU, GPU, RAM, SSD/HDD.

Algoritmi Avanzati: Valutazione hardware raffinata:

RAM: Punteggio combinato (70% dimensione, 30% velocità).

Storage: Distinzione e bonus prestazionale per SSD NVMe, SSD SATA e HDD.

CPU/GPU: Punteggi basati su core, thread, frequenza, architettura e generazione.

2. 🛡️ Analisi Sicurezza e Ottimizzazioni di Sistema
Verifica critica delle configurazioni di sicurezza e ottimizzazione di Windows:

Sicurezza: Controllo dello stato del TPM 2.0 e dell'attivazione di Secure Boot.

Ottimizzazioni: Analisi di parametri chiave come:

Stato di CPU Parking.

Stato di GPU Hardware Scheduling.

Configurazione HPET.

Analisi del Piano di Alimentazione (Power Plan) e stato della Xbox Game Bar.

3. 🌍 Usabilità e Interfaccia Utente (UI)
Interfaccia Multilingua: Rilevamento automatico della lingua (Italiano/Inglese) con dizionario completo per tutti i testi e messaggi.

Affidabilità: Gestione robusta degli errori, scansione non bloccante per mantenere la UI reattiva, e gestione ottimizzata della memoria.

Aggiornamenti: Sistema di aggiornamento integrato per il download incrementale dei dati online, con fallback in assenza di connessione.


1. **Correzione Rilevamento Disco Primario - Gaming PC Check**:
   - Problema Risolto
   - Issue: Lo script identificava erroneamente il disco primario del sistema operativo come HDD invece che SSD, causando una valutazione inaccurata delle prestazioni

2. **📈 Miglioramenti**:
   - Affidabilità: Minor dipendenza da strutture WMI complesse
   - Precisione: Rilevamento corretto SSD/HDD per disco sistema
   - Punteggio accurato: Bonus SSD applicati correttamente (+3 punti)
   - Compatibilità: Funziona su diverse configurazioni hardware

1. **Riconoscimento GPU integrata completo**:
   - Intel: UHD Graphics, HD Graphics, Iris Xe
   - AMD: Radeon Graphics, Vega Graphics, RX serie integrata
   - Pattern di riconoscimento più accurati

2. **Logica di selezione GPU primaria**:
   - Priorità alle GPU dedicate
   - Tra le dedicate, sceglie quella con punteggio più alto
   - Solo se non ci sono dedicate, usa le integrate

3. **Punteggi appropriati per GPU integrate**:
   - Punteggio massimo limitato per GPU integrate
   - Bonus per GPU integrate più potenti (Iris Xe, Radeon 680M/780M)
   - Stima VRAM realistica basata sulla RAM di sistema

4. **Visualizzazione chiara**:
   - Mostra esplicitamente "GPU PRIMARIA"
   - Elenca le altre GPU rilevate separatamente
   - Calcola il punteggio complessivo SOLO con la GPU primaria

5. **Suggerimenti contestuali**:
   - Suggerisce upgrade GPU solo per GPU dedicate con punteggio basso
   - Non suggerisce upgrade per GPU integrate (sarebbe inutile)

Ora lo script:
- ✅ Rileva correttamente tutte le GPU (Intel, AMD, NVIDIA)
- ✅ Distingue tra integrate e dedicate
- ✅ Seleziona automaticamente la GPU primaria attiva
- ✅ Calcola il punteggio solo sulla GPU primaria
- ✅ Mostra tutte le GPU rilevate ma usa solo quella principale per il voto.
### 🚀 New Features

#### **Real-time CPU Parking Status Monitor**
- **Added visual indicator** for CPU core parking status in the main interface
- **Color-coded display**: 
  - 🟢 **GREEN BOLD** "CPU Unparked" when core parking is disabled
  - 🔴 **RED** "CPU Parked" when core parking is enabled
- **Automatic status detection** from Windows registry settings
- **Real-time updates** when:
  - Application starts
  - Boost mode is activated/deactivated
  - Language is changed

### 🔧 Technical Improvements

#### **UI/UX Enhancements**
- **New UI element** positioned below CPU usage monitor
- **Dynamic text updates** based on current system state
- **Multi-language support** with translations for both Italian and English
- **Automatic layout adjustment** with increased window height to accommodate new element

#### **Code Architecture**
- **New utility functions**:
  - `Get-CPUParkingStatus()` - Reads current CPU parking state from registry
  - `Update-CPUParkingIndicator()` - Updates visual indicator based on system state
- **Enhanced event handling** with status updates on:
  - Boost toggle operations
  - Language selection changes
  - Application initialization

### 🌐 Localization Updates

#### **New Translation Keys**
- `CPUParkingDisabled`: "CPU Sparcheggiata" (IT) / "CPU Unparked" (EN)
- `CPUParkingEnabled`: "CPU Parcheggiata" (IT) / "CPU Parked" (EN)

### 📊 System Integration

#### **Registry Monitoring**
- **Direct registry polling** of CPU power management settings
- **Error handling** for registry access issues
- **Cross-version compatibility** with Windows power management schemas

### 🎯 User Benefits

- **Instant visual feedback** on CPU optimization state
- **Clear status indication** without needing to check system settings
- **Enhanced transparency** of what the boost feature actually does
- **Better user confidence** in optimization effectiveness

### 🔄 Compatibility

- **Windows Versions**: Windows 7, 8, 10, 11
- **Architectures**: x64, x86
- **Requirements**: Administrator privileges (maintained from previous versions)

---

### 📝 Notes for Users

The CPU parking status indicator provides real-time feedback on whether your CPU cores are currently parked (power-saving mode) or unparked (full performance mode). This helps users verify that the performance optimizations are actually taking effect.

### 🔍 Technical Details

The feature monitors the registry key:
`HKLM\SYSTEM\CurrentControlSet\Control\Power\PowerSettings\54533251-82be-4824-96c1-47b60b740d00\0cc5b647-c1df-4637-891a-dec35c318583`

**Values:**
- `ValueMax = 0` → CPU Unparked (Performance Mode)
- `ValueMax = 1` → CPU Parked (Power Saving Mode)

---

*For full documentation and source code, visit our [GitHub repository](https://github.com/ilborga70)*

---

**SCL Gaming Boost** is a lightweight yet powerful Windows utility designed to maximize your in-game performance. It intelligently disables non-essential services, halts background telemetry, and applies system-level tweaks to free up resources and reduce latency, giving you a smoother and more responsive gaming experience.

> **Disclaimer**: You can check suspicious files for malicious programs free of charge using the Dr.Web online file scanner: [https://vms.drweb-av.it/scan\_file/](https://vms.drweb-av.it/scan_file/)

-----

## 🧪 Benchmark: Sniper Elite V2 Remastered

**Windows 11 Game Mode vs. Game Mode + SCL Gaming Boost**

We ran two benchmark tests using identical hardware and graphics settings. The only difference? One test used Windows 11's built-in Game Mode, while the other added **SCL Gaming Boost** on top.

### 🖥️ Test Setup

  - **CPU**: Intel Core i5-13600KF
  - **GPU**: NVIDIA GeForce RTX 4080
  - **RAM**: 64 GB
  - **Resolution**: 2560 x 1080
  - **Graphics Settings**: ULTRA preset, V-Sync OFF, Supersampling OFF

-----

### 📊 Performance Comparison

| Metric | Game Mode Only | Game Mode + SCL Gaming Boost |
|----------------------|----------------|-------------------------------|
| **Average FPS** | 710.9 | 730.3 |
| **Minimum FPS** | 226.4 | 270.2 |
| **Maximum FPS** | 1378.4 | 1342.3 |
| **Avg. Frame Time** | 1.407 ms | 1.369 ms |
| **Min. Frame Time** | 0.725 ms | 0.745 ms |
| **Max. Frame Time** | 4.416 ms | 3.700 ms |

### 🧠 Analysis & Takeaways

  - ✅ **+2.7% Average FPS**: A solid increase in overall framerate.
  - 🚀 **+19.3% Minimum FPS**: A massive improvement in stability, reducing stutters and dips.
  - ⚡ **Lower Average Frame Time**: Snappier, more immediate responsiveness.
  - 📉 **Reduced Max Frame Time**: Smoother frame pacing and less noticeable stutter.

**Final Verdict**: **SCL Gaming Boost** delivers measurable performance gains, especially in minimum FPS and frame time consistency, making it ideal for competitive or high-refresh-rate gaming.

-----

## 🎮 Key Features

  - **🎯 Customizable Boost Modes**:
      - **FPS Boost**: Maximizes your frame rate by disabling all non-critical services and applying aggressive performance tweaks.
      - **Streaming Mode**: Optimizes your system for smooth streaming by keeping essential network and encoding-related services active while boosting game performance.
      - **Standard Mode**: Safely and completely restores your system to its original state by loading a **backup of your personal settings**, not just applying generic default values.
  - **✨ One-Click Optimization**: A simple, intuitive interface to apply and revert all changes.
  - **💾 Automatic Preference Saving**: The tool remembers your chosen language and optimization settings between sessions.
  - **🌐 Multi-Language Support**: Switch between languages on the fly.
  - **🔄 Quick System Restart**: A convenient button to restart your PC and ensure all tweaks are applied correctly.
  - **📝 Detailed Operation Log**: A `SCLGamingBoost.log` file is generated in your user profile to track all actions taken by the tool.

-----

## 🛠️ How to Use

1.  **Download** the latest `.exe` from the [Releases page](https://www.google.com/search?q=https://github.com/ilborga70/SCL-Gaming-Boost/releases).
2.  **Run as Administrator**. This is required to modify system services and registry settings.
3.  **Select Your Language and Optimizations** from the main panel.
4.  **Choose a Boost Mode** from the dropdown menu (`FPS Boost`, `Streaming Mode`).
5.  Click the **Start Boost** button.
6.  **(Recommended)** Restart your system to ensure all changes take effect.
7.  To revert, simply open the tool and click **Stop Boost**.

-----

## ✨ Optimizations at a Glance

This version introduces a series of powerful optimizations, each of which can be enabled or disabled from the user interface.

| Optimization | Detailed Description |
|---|---|
| 🔕 **Disable Windows Notifications** | Disables all system notifications to prevent annoying pop-ups and micro-stuttering that can disrupt gaming fluidity.
| 🌐 **Disable Network Throttling** | Prevents the system from throttling your network card's bandwidth to save power. Crucial for preventing lag and latency spikes in online games.
| 🧹 **Clear DNS Cache** | Flushes the system's DNS cache to resolve potential connection issues and improve response times (ping) with game servers.
| 💾 **Disable Hibernation** | Disables the hibernation feature to free up gigabytes of valuable disk space (by deleting `hiberfil.sys`) and reduce overall system load.
| 🎯 **Disable Mouse Acceleration** | Provides a true 1:1 mouse response by removing pointer acceleration at the OS level. Essential for precision in FPS games and e-sports.
| 🔄 **Disable Windows Update** | Temporarily stops the Windows Update service from downloading and installing updates in the background, which consumes resources and causes FPS drops.

-----

## ⚙️ How It Works: The Technical Details

The tool temporarily modifies system settings to maximize performance. Here’s a look under the hood:

  - **Service Management**: Stops and disables a curated list of background services and telemetry activities that consume CPU, memory, and network cycles.
  - **CPU Management**: Disables CPU "Core Parking" to ensure all cores are active and ready. It also activates the "Ultimate Performance" power plan to ensure the processor runs at its full potential without throttling.
  - **System & Memory Tweaks**: Applies registry modifications to optimize thread scheduling, memory management (by prioritizing system cache and keeping drivers in RAM), and visual effects.
  - **Game Bar & DVR Removal**: Disables services and registry keys related to the Windows Game Bar and background recording features that can impact performance.

### Disabled Services

The following services are disabled in `FPS Boost` mode:

```
SysMain (Superfetch)
WSearch (Windows Search)
DiagTrack (Connected User Experiences and Telemetry)
Fax
Spooler (Print Spooler)
WMPNetworkSvc (Windows Media Player Network Sharing)
XblGameSave (Xbox Live Game Save)
BluetoothSupportService
RemoteRegistry
PhoneSvc
```

### Disabled Scheduled Tasks

Key telemetry and data collection tasks are disabled:

```
Microsoft\Windows\Application Experience\ProgramDataUpdater
Microsoft\Windows\Autochk\Proxy
Microsoft\Windows\Customer Experience Improvement Program\Consolidator
Microsoft\Windows\Customer Experience Improvement Program\UsbCeip
```

### Core Registry Tweaks

| Registry Key | Value Set | Description |
|---|---|---|
| `HKLM\SOFTWARE\Policies\Microsoft\Windows\DataCollection` | `AllowTelemetry: 0` | Disables core system telemetry. |
| `HKLM\SYSTEM\CurrentControlSet\Control\PriorityControl` | `Win32PrioritySeparation: 26` | Optimizes CPU thread priority for foreground applications (games). |
| `HKCU\Software\Microsoft\Windows\CurrentVersion\Explorer\VisualEffects` | `VisualFXSetting: 2` | Disables unnecessary visual effects like animations for raw performance. |
| `HKCU\SOFTWARE\Microsoft\Windows\CurrentVersion\GameDVR` | `AppCaptureEnabled: 0` | Disables the native Windows game recording feature. |
| `HKCU\SOFTWARE\Microsoft\GameBar` | `ShowStartupPanel: 0` | Prevents the Game Bar from appearing. |
| `HKLM\SYSTEM\CurrentControlSet\Control\Session Manager\Memory Management` | `LargeSystemCache: 1` | Prioritizes the system file cache for faster I/O operations. |
| `HKLM\SYSTEM\CurrentControlSet\Control\Session Manager\Memory Management` | `DisablePagingExecutive: 1` | Forces drivers and kernel code to remain in physical RAM, preventing paging and improving responsiveness. |

-----

## ⚠️ Important Information

  - **Run as Administrator**: This script **must** be run with administrator permissions to apply the necessary changes to system services and the registry.
  - **Safe Restore**: The "Standard" mode restores your PC to its **exact original state** by using a backup file created before the first boost. This ensures a 100% safe and reversible process.
  - **Compatibility**: Designed and tested for **Windows 10 and 11**. It may not function correctly on earlier versions.

## 📦 Requirements

  - **OS**: Windows 10 or higher
  - **PowerShell**: Version 5.0+ (pre-installed on modern Windows)
  - **Permissions**: Administrator rights

-----

## 📜 License

This project is licensed under the **MIT License**. Feel free to use, modify, and distribute it. See the `LICENSE` file for more details.

-----

## 👤 About the Developer

**ilborga70** — Gamer, Developer, and Serial Optimizer.

  - 📧 **Email**: [borgaccino@gmail.com](mailto:borgaccino@gmail.com)
  - 🔗 **GitHub Profile**: [https://github.com/ilborga70](https://github.com/ilborga70)



🔗 [GitHub Profile](https://github.com/ilborga70)
