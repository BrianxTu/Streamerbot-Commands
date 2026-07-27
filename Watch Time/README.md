# REQUIRED

**Uptime is required** for functionality.

---

# !watchtime

A utility command that reports how long a user has watched the stream. Watchtime is tracked continuously in the background, and the command displays the accumulated total. It supports self‑lookup, targeting another user, a **full** mode for detailed output, and a watchtime **leaderboard**.

## Usage
`!watchtime`  
`!watchtime full`  
`!watchtime <target>`  
`!watchtime <target> full`  
`!watchtime leaderboard`  
Aliases: `lb`, `lead`, `leader`, `leaders`

- Without a target, the command reports **your** watchtime.  
- With a target, it reports **their** watchtime.  
- Adding **full** shows a detailed breakdown (years, months, weeks, days, hours, minutes, seconds).  
- Without **full**, the output is shortened to the first one or two time units.  
- Using a leaderboard alias displays the top watchtime users.

## Leaderboard
If enabled, the leaderboard shows the top watchers (default: top 5).  
Each entry uses a compact format such as `1y 2mo 3d 4h`.

## Example
`!watchtime`  
→ `@UserName, you have watched for 3 months & 2 weeks.`

`!watchtime CoolViewer full`  
→ `@UserName, @CoolViewer has watched for 1 year, 4 months, 2 weeks & 6 days.`

`!watchtime leaderboard`  
→ `Watchtime Leaderboard: 1. @ViewerA - 2y 3mo, 2. @ViewerB - 1y 5mo, ...`

## Background Tracking
Watchtime is updated automatically by background watchers. The command simply reads and formats the stored values.

## Customization
Adjust message templates, leaderboard size, or time formatting by modifying the corresponding variables in the script.

Made by **BrianTU**

---

# !checkin

A utility command that marks a user as “checked in,” allowing their active watchtime to begin tracking. The script can be triggered either by a chat command or by a channel point redemption. It verifies that the stream is online, checks whether the user is already checked in, and updates their watchtime start timestamp.

## Usage
`!checkin`  
(or via channel point redemption)

- If the stream is offline, the command returns an offline message.  
- If the user is already checked in, it notifies them.  
- Otherwise, it records the current time as their watchtime start.

## Example
`!checkin`  
→ `@UserName, you are now checked in.`

If already checked in:  
→ `@UserName, you are already checked in.`

If the stream is offline:  
→ `The stream is currently offline.`

## Background Behavior
Checking in sets the user’s `watchStart` value, which is used by the watchtime system to calculate active viewing time.

## Customization
Modify the message templates (`alreadyMessage`, `startedMessage`, `offlineMessage`) to change how responses appear.

Made by **BrianTU**