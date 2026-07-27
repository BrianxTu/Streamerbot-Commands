# !shoutout

A cross‑platform shoutout command that highlights a creator and links to their channel on Twitch, YouTube, or Kick. You can optionally broadcast the shoutout to **cross** platforms at once.

## Usage
`!shoutout <target>`  
`!shoutout <target> cross` → sends the shoutout to Twitch, YouTube, and Kick.

The script cleans the target name, builds the correct profile link, and formats the shoutout using the platform’s message template.

### Twitch‑specific behavior
If available, the shoutout includes the last game the user streamed. Otherwise, it uses the fallback Twitch message.

## Example
`!shoutout CoolStreamer`  
→ `A huge shoutout to @CoolStreamer! They were last seen playing Game Name. Check them out! https://www.twitch.tv/CoolStreamer`

`!shoutout CoolStreamer all`  
→ Sends the shoutout to **cross** supported platforms.

## Customization
Edit the `shoutoutData` dictionary to adjust message templates or link bases.

Made by **BrianTU**