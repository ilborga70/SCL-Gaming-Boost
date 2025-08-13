# 🎮 SCL Gaming Boost

![Platform](https://img.shields.io/badge/platform-Windows-blue)
![PowerShell](https://img.shields.io/badge/language-PowerShell-lightgrey)
![Status](https://img.shields.io/badge/status-Active-brightgreen)

**SCL Gaming Boost** è un utility avanzata per Windows pensata per i gamer più esigenti. Ottimizza il sistema operativo con un solo click, disattivando servizi superflui, riducendo la telemetria e applicando tweak intelligenti per migliorare le prestazioni in gioco.

<img width="2560" height="1080" alt="Sniper Elite V2 Remastered Windows 11 + SCL Gaming Boost + Game Mode" src="https://github.com/user-attachments/assets/29251245-fccd-44c3-a0ac-e7a580bd5c9c" />

---

<img width="2560" height="1080" alt="vms drweb-av" src="https://github.com/user-attachments/assets/5a887536-e2f3-403d-89f7-7af378ff70f1" />

https://vms.drweb-av.it/scan_file/?utm_medium=glavnaya&utm_source=drweb_site&utm_campaign=scanfile

---

# 🖥️ 1. Scarica e avvia il programma
- Vai alla pagina GitHub del progetto: https://github.com/ilborga70/SCL-Gaming-Boost/releases/tag/0.9.0.0
- Scarica il file SCL Gaming Boost.exe.
- Avvia l'applicazione come amministratore (clic destro → "Esegui come amministratore").

🎮 2. Scegli la modalità di Boost
Nella GUI troverai tre profili:
- FPS Boost: massimizza le prestazioni nei giochi.
- Streaming Mode: bilancia prestazioni e stabilità per lo streaming.
- Standard: ottimizzazioni leggere per uso quotidiano.

Seleziona quello più adatto alle tue esigenze.

⚙️ 3. Applica il Boost
- Premi il pulsante "Boost" per attivare le ottimizzazioni.
- Il programma disattiverà servizi inutili, modificherà il registro e fermerà task pianificati.
- Lo stato delle ottimizzazioni sarà visibile in tempo reale.

🔁 4. Riavvia il sistema (opzionale)
- Dopo aver applicato il Boost, puoi cliccare su "Restart" per riavviare il PC e rendere effettive tutte le modifiche.

📝 5. Controlla i log
- Tutte le operazioni vengono salvate in un file .log nella cartella del programma, utile per monitoraggio e debugging.

---

## 🚀 Funzionalità

- ✅ **Modalità Boost personalizzabile**  
  Attiva ottimizzazioni mirate per il gaming, lo streaming o l’uso quotidiano.

- 🎯 **Profili selezionabili**  
  - FPS Boost  
  - Streaming Mode  
  - Standard

- 📊 **Controllo in tempo reale**  
  Visualizza lo stato attivo/inattivo direttamente dalla GUI.

- 🧠 **Salvataggio automatico delle preferenze**  
  Il programma ricorda le tue ultime impostazioni e lo stato del Boost.

- 🔁 **Riavvio rapido del sistema**  
  Pulsante dedicato per riavviare Windows in modo sicuro.

- 📝 **Log dettagliato delle operazioni**  
  Tutte le azioni vengono registrate in un file `.log` per monitoraggio e debugging.

---

## 🛡️ Ottimizzazioni applicate

### 🔧 Servizi disattivati durante il Boost

| Servizio                  | Descrizione                                      |
|---------------------------|--------------------------------------------------|
| `SysMain`                 | Ottimizzazione automatica del sistema (Superfetch) |
| `WSearch`                 | Indicizzazione file e ricerca                    |
| `DiagTrack`               | Telemetria e tracciamento diagnostico           |
| `Fax`                     | Servizio fax (raramente usato)                  |
| `Spooler`                 | Gestione stampa                                 |
| `WMPNetworkSvc`           | Condivisione multimediale di Windows Media Player |
| `XblGameSave`             | Salvataggi cloud Xbox                           |
| `BluetoothSupportService`| Supporto Bluetooth                               |
| `RemoteRegistry`          | Accesso remoto al registro                      |
| `PhoneSvc`                | Servizi legati alla telefonia                   |

### 📅 Attività pianificate disattivate

| Attività                                                                 |
|--------------------------------------------------------------------------|
| `ProgramDataUpdater` – Esperienza applicazioni                          |
| `Proxy` – Autochk                                                        |
| `Consolidator` – Programma miglioramento esperienza cliente             |
| `UsbCeip` – Telemetria USB                                               |

---

## 🧠 Modifiche al Registro di Sistema

| Chiave di registro                                                                 | Valore impostato | Descrizione                                                                 |
|------------------------------------------------------------------------------------|------------------|-----------------------------------------------------------------------------|
| `HKLM\SOFTWARE\Policies\Microsoft\Windows\DataCollection\AllowTelemetry`           | `0`              | Disattiva la telemetria                                                     |
| `HKLM\SYSTEM\CurrentControlSet\Control\PriorityControl\Win32PrioritySeparation`   | `26`             | Ottimizza la priorità dei thread                                            |
| `HKCU\Software\Microsoft\Windows\CurrentVersion\Explorer\VisualEffects\VisualFXSetting` | `2`         | Disattiva effetti visivi                                                    |
| `HKCU\SOFTWARE\Microsoft\Windows\CurrentVersion\GameDVR\AppCaptureEnabled`        | `0`              | Disattiva la registrazione automatica dei giochi                           |
| `HKCU\SOFTWARE\Microsoft\GameBar\ShowStartupPanel`                                | `0`              | Nasconde il pannello Game Bar all’avvio                                     |
| `HKCU\SOFTWARE\Microsoft\GameBar\AutoGameModeEnabled`                             | `0`              | Disattiva Game Mode automatico                                              |
| `HKCU\SOFTWARE\Microsoft\GameBar\AllowAutoGameMode`                               | `1`              | Consente Game Mode manuale                                                  |
| `HKLM\SYSTEM\CurrentControlSet\Control\Session Manager\Memory Management\LargeSystemCache` | `1`      | Ottimizza la cache di sistema                                               |
| `HKLM\SYSTEM\CurrentControlSet\Control\Session Manager\Memory Management\DisablePagingExecutive` | `1` | Mantiene i driver in RAM per prestazioni migliori                          |

> 🔁 Tutte le modifiche vengono **ripristinate automaticamente** quando il Boost viene disattivato.

---

## 📦 Distribuzione

Il programma è disponibile come **file eseguibile** per Windows. Nessuna installazione richiesta: basta avviarlo con privilegi amministrativi.

> ⚠️ **Nota:** Alcune ottimizzazioni richiedono diritti di amministratore. Assicurati di eseguire il programma come _Administrator_.

---

## 🛠️ Requisiti

- Windows 10 o superiore  
- PowerShell 5.0+  
- Privilegi amministrativi

---

## 📁 File generati

- `SCLGamingBoost.log` – Registro delle operazioni  
- `SCLGamingBoost.settings` – Preferenze utente salvate

---

## 💬 Feedback & Contributi

Hai idee per nuove funzionalità? Vuoi contribuire al progetto? Apri una issue o invia una pull request!

---

## 📜 Licenza

Questo progetto è distribuito sotto licenza **MIT**. Puoi usarlo, modificarlo e distribuirlo liberamente.

---


**ilborga70** – Gamer, sviluppatore, ottimizzatore seriale.  
Per contatti o collaborazioni: [borgaccino@gmail.com]
