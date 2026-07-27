# !title

A utility command that displays the current stream title. The script retrieves the active broadcast’s title from the platform where the command was triggered and sends it to chat. If no title is found, it returns a simple fallback message.

## Usage
`!title`

- The command reports the current stream title.  
- If the title cannot be retrieved, it displays a “no title found” message.

## Example
`!title`  
→ `The current stream title is: Cozy Vibes & Chill Chat`

If no title is available:  
→ `The current stream title is: no title found!`

## Customization
Edit `finalMessageBase` or `noTitle` to change how the output appears.

Made by **BrianTU**