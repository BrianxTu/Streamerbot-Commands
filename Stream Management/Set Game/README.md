# !setgame

A utility command that updates the stream’s category/game on Twitch, YouTube, or Kick. The script reads the raw input text, sends the update request to the correct platform, and reports whether the update succeeded.

## Usage
`!setgame <category or game name>`

- The command updates the stream category on the platform where it was triggered.  
- If the update succeeds, it sends a success message.  
- If the update fails, it sends a failure message.

## Example
`!setgame Just Chatting`  
→ `Category updated successfully.`

If the update fails:  
→ `Failed to update the category.`

## Customization
Edit `successMessage` or `failMessage` to change how responses appear.

Made by **BrianTU**