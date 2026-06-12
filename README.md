
# Windows Security Monitor Pipeline 

A real-time security integration pipeline that monitors Windows Security Event logs for failed login attempts (Event ID 4625) and alerts users immediately via Telegram.

## Features
- **Live Auditing:** Directly interfaces with the Windows Event Log API to scan for unauthorized access attempts in real-time.
- **Instant Alerts:** Bridges system-level events to your pocket using the Telegram Bot API.
- **Forensic Context:** Captures key indicators of compromise, such as the targeted account name and the source IP/workstation.

##  Tech Stack
- **Language:** Python
- **API Integration:** `win32evtlog` (Windows OS), `requests` (Telegram API)

##  How to Use
1. Clone this repository to your local machine.
2. Obtain a Telegram Bot Token from @BotFather.
3. Update `TOKEN` and `CHAT_ID` in `real_windows_defender.py`.
4. **Crucial:** Execute the script using an **Administrator-level Command Prompt** to grant the necessary read privileges to the Windows Security vault.
