# !uptime

A utility command that reports how long the stream has been live. Uptime is tracked automatically by background watchers that record when the stream goes online and offline across all supported platforms. The command reads that stored start time, calculates the current uptime, formats it, and sends the result to chat.

## Usage
`!uptime`  
`!uptime full`

- Without **full**, the command shows a shortened uptime (first one or two time units).  
- With **full**, it shows a detailed breakdown (years, months, weeks, days, hours, minutes, seconds).  
- If the stream is offline, the command returns an offline message.

## Example
`!uptime`  
→ `Uptime: 3 hours & 12 minutes.`

`!uptime full`  
→ `Uptime: 1 day, 4 hours, 22 minutes & 10 seconds.`

If offline:  
→ `The stream is currently offline.`

## Background Tracking
Two background watchers update the global `streamStart` value whenever the stream goes online or offline. The command simply reads that timestamp and formats the elapsed time.

## Customization
Modify `uptimeMessage`, `offlineMessage`, or adjust `FormatTime` function to adjust time units or formatting rules.

Made by **BrianTU**