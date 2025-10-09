## v2.4.0 - 2025-10-10

## ![SCL Gaming Boost v2 4 0+](https://github.com/user-attachments/assets/acceabd9-f226-4d15-936c-650b06791c0f)

### 🎮 Miglioramenti principali

- **Correzione rilevamento disco primario**: ora distingue correttamente tra SSD e HDD per un punteggio più accurato.
- **Riconoscimento GPU migliorato**:
  - Supporto completo per GPU Intel (UHD, HD, Iris Xe) e AMD (Radeon, Vega, RX integrati).
  - Priorità alle GPU dedicate con punteggio più alto.
  - Stima realistica della VRAM per GPU integrate.
- **Logica di punteggio aggiornata**:
  - Bonus per SSD (+3 punti).
  - Punteggio massimo limitato per GPU integrate, con eccezioni per modelli avanzati come Iris Xe e Radeon 780M.
- **Visualizzazione chiara della GPU**:
  - Mostra “GPU PRIMARIA” e le altre separatamente.
  - Solo la GPU primaria influisce sul punteggio.
- **Suggerimenti contestuali per upgrade**:
  - Raccomandazioni solo per GPU dedicate con punteggio basso.

---

### 🧠 Novità: Monitor stato CPU Parking in tempo reale

- Indicatore visivo nella UI:
  - 🟢 “CPU Unparked” (modalità prestazioni)
  - 🔴 “CPU Parked” (modalità risparmio energetico)
- Aggiornamento dinamico all’avvio, al cambio lingua o al toggle boost.
- Rilevamento via registro compatibile con tutte le versioni di Windows.

---

### 🛠 Ottimizzazioni tecniche

- **UI/UX**:
  - Nuovo elemento sotto il monitor uso CPU.
  - Supporto multilingua (italiano + inglese).
- **Architettura del codice**:
  - Nuove funzioni: `Get-CPUParkingStatus()` e `Update-CPUParkingIndicator()`.
  - Migliorata la gestione degli eventi per toggle boost e cambio lingua.

---

### 📊 Benchmark: Sniper Elite V2 Remastered

| Metica                | Solo Game Mode | Game Mode + SCL Boost |
|----------------------|----------------|------------------------|
| FPS Medio            | 710.9          | 730.3                  |
| FPS Minimo           | 226.4          | 270.2                  |
| FPS Massimo          | 1378.4         | 1342.3                 |
| Frame Time Medio     | 1.407 ms       | 1.369 ms               |
| Frame Time Massimo   | 4.416 ms       | 3.700 ms               |

**Conclusione**: +2.7% FPS medio, +19.3% FPS minimo, maggiore fluidità.

---

### 🌟 Modalità Boost

- **FPS Boost**: ottimizzazioni aggressive per le prestazioni.
- **Streaming Mode**: mantiene servizi essenziali per lo streaming.
- **Standard Mode**: ripristina il sistema usando il backup personale.

---

### 🔧 Ottimizzazioni disponibili

| Ottimizzazione              | Descrizione |
|----------------------------|-------------|
| 🔕 Disattiva notifiche      | Evita popup e micro-scatti. |
| 🌐 Disattiva throttling rete| Migliora la latenza online. |
| 🧠 Pulisci cache DNS        | Migliora la risposta dei server. |
| 💾 Disattiva ibernazione    | Libera spazio e riduce carico. |
| 🎯 Disattiva accelerazione mouse | Precisione 1:1. |
| 🔄 Disattiva Windows Update | Evita cali di FPS in background. |

---

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
