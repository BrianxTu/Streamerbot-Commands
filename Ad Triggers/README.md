# Ad Triggers  
A Twitch-only StreamerBot feature that provides ad warnings, formatted ad messages, and welcome-back notification for viewers returning from ads.

This system uses StreamerBot sub-actions combined with C# logic to deliver accurate timing, readable messages, and consistent behavior.

---

## Feature Included  
- Ad Warning + Message + Welcome Back

---

## Ad Warning  
Sends a warning when Twitch is about to run an ad.

**Description:**  
Triggers once per minute for up to the 5-minute warning Twitch provides to mods and the broadcaster.

---

## Ad Message  
Displays a readable message showing the ad length.

**Description:**  
Ad duration is formatted in C# and returned as a variable that can be used in StreamerBot messages.

---

## Welcome Back  
Greets viewers returning from an ad. Shares the same trigger as Ad Message

**Description:**  
Uses the formatted ad duration to send a welcome-back message once the ad ends.
