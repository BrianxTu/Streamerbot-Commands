# Uptime Command  
A StreamerBot command that displays how long the stream has been live.

Works across all platforms StreamerBot supports, with Twitch offering the strongest support.

---

## Command Included  
- Uptime

---

## Uptime  
Shows how long the stream has been running.

**Command:**  
`!uptime <full>`

**Description:**  
Returns the current stream uptime.  
Adding `full` displays the complete uptime down to seconds.

**Notes:**  
- Uptime is required for the Watchtime command

---

## Handlers  
These handlers track the stream's status and are required for uptime and watchtime accuracy.

**Stream Online Record**  
Records when the stream goes live.

**Stream Offline End**  
Records when the stream goes offline.
