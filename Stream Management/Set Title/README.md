# !settitle

A utility command that updates the stream title on Twitch, YouTube, or Kick. The script reads the raw input text, sends the update request to the correct platform, and reports whether the update succeeded.

## Usage
`!settitle <new title>`

- The command updates the stream title on the platform where it was triggered.  
- If the update succeeds, it sends a success message.  
- If the update fails, it sends a failure message.

## Example
`!settitle Cozy Vibes & Chill Chat`  
→ `Title updated successfully.`

If the update fails:  
→ `Failed to update the stream title.`

## Customization
Edit `successMessage` or `failMessage` to change how responses appear.

Made by **BrianTU**