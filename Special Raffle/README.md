# Raffle System

A full multi‑platform raffle system supporting Twitch, YouTube, and Kick.  
Moderators can create, end, draw, reopen, reset, and dump raffles.  
Viewers can join active raffles and check the current status.

Made by **BrianTU**

---

# Commands

## Viewer Commands
`!sjoin`  
`!sj`  
Join the active raffle.  
If the raffle is sub‑only or platform‑restricted, the system will notify you.

`!rafflestatus`  
`!rfs`  
Shows the current raffle status, including prize, participant count, platform rules, and winners (if any).

---

## Moderator Commands  
All moderator commands use the main raffle prefix:

`!sraffle`  
`!srf`

Each requires a **sub‑command**.

### Create  
`!sraffle create <allPlatforms> <subOnly> <prize...>`  
Aliases: `new`, `start`

Starts a new raffle.

- `allPlatforms` — `true/false` or `yes/no/1/0`  
- `subOnly` — `true/false` or `yes/no/1/0`  
- `prize` — any text (multi‑word supported)

Example:  
`!sraffle create 1 0 End Stream Early`

---

### End  
`!sraffle end`  
Alias: `stop`

Ends the raffle and locks entries.

---

### Draw  
`!sraffle draw <winners>`  
Aliases: `pick`

Draws the specified number of winners.  
Weighted entries apply automatically.

Example:  
`!sraffle draw 3`

---

### Reopen  
`!sraffle reopen <clearEntries>`  
Alias: `resume`

Reopens a closed raffle.

- `clearEntries` — `true/false` or `yes/no/1/0`  
  - `true` clears entries, join count, and winners  
  - `false` keeps everything

Example:  
`!sraffle reopen true`

---

### Reset  
`!sraffle reset`  
Alias: `clear`

Fully resets all raffle data.  
Only allowed after the raffle has ended.

---

### Dump  
`!sraffle dump`  
Alias: `save`  

Outputs all raffle variables to the **log** for inspection.  
Useful for troubleshooting, verifying state or saving.

---

# Features

### Weighted Entries (Changeable in code)
- Normal viewer: **1 entry**  
- Subscriber: **2 entries**  
- Moderator: **1 entry**

### Platform Restrictions  
Raffles can be:
- Open to **all platforms**, or  
- Restricted to the **platform that created the raffle**

### Sub‑Only Mode  
If enabled, only subscribers may join.

### Winner Storage  
Winners are stored and shown in status until cleared or reset.

### Logging  
All errors, dumps, and unknown platform messages are logged.

---

# Status Output

`!rafflestatus` shows:

- Raffle state (Open/Closed)  
- Prize  
- Participant count  
- Platform rules  
- Sub‑only flag  
- Winner list (if any)

Example:  
`Raffle: Open | Prize: End Stream Early | Participants: 12 | Platform: All | Sub-Only: Yes`

---

# Notes

- All commands are under one command entry. IF YOU CHANGE THE COMMANDS, CHANGE THEM IN THE CSHARP OR IT WILL NOT WORK!
- True/False and aliases are changable at the top of the CSharp.
- Raffle command sub-commands are changeable at the top of the CSharp.
- Moderator only commands are changeable at the top of the CSharp.
- All messages are organized at the top of the csharp to easily change for language support.
