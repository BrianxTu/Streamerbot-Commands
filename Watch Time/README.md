# Watchtime Command  
A StreamerBot command that tracks how long a user has watched the stream. This system **requires the Uptime command** to function and provides both personal watchtime and optional leaderboard output.

Fully customizable through C# and works across all platforms StreamerBot supports.

---

## Command Included  
- Watchtime  
- Check-in

---

## Watchtime  
Displays how long a user has watched the stream.

**Command:**  
`!watchtime <leaderboard>`  
`!watchtime <full/target> <full>`

**Description:**  
Returns the watchtime for the user or a specified target.  
Can be used with or without a target or leaderboard.

**Notes:**  
- Leaderboard is optional and toggleable

---

## Check-in  
Manually checks a user in for watchtime tracking.

**Command:**  
`!checkin`

**Description:**  
Forces a check-in for the user. 

---

## Handlers

**Present Viewers Watchtime**  
Tracks when a user joins or leaves, force starting or force saving when needed.

**Offline Watchtime Cleanup**  
Force saves remaining watchtime if the stream goes offline.
