# Ad Warning

A passive Twitch‑only system that sends periodic warnings before an ad break begins.

## Behavior
- Sends a countdown‑style warning message before ads begin.  
- Can be configured to run every minute, up to five minutes before the ad break.  
- Only triggers on Twitch, since ad timing data is Twitch‑specific.

## Example
→ `Ads starting in 3 minutes — Ad Warning`  
→ `Ads starting in 1 minute - Ad Warning`

## Customization
Adjust the warning interval or message text to fit your stream’s style.

Made by **BrianTU**

---

# Ad Message + Welcome Back — README

A shared action used during ad breaks.

## Behavior
1. Converts the ad length (in seconds or milliseconds) into a readable time string.  
2. Sends a Twitch chat message announcing the ad break.  
3. Waits for the full ad duration.  
4. Sends a welcome‑back message when the ad ends.

This action is used by both the automated ad‑warning system and any manual ad‑triggering workflows.

## Example
→ `We’re taking a break. See you in 90 seconds!`  
(wait for ad duration)  
→ `Welcome back from the ad break!`

## Customization
Edit the ad‑start message, the welcome‑back message, or the formatting logic.

Made by **BrianTU**