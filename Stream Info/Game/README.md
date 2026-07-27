# !game — README

A utility command that displays the current stream category/game. The script retrieves the active broadcast’s game/category from the platform where the command was triggered and sends it to chat. If no category is found, it returns a simple fallback message.

## Usage
`!game`

- The command reports the current stream game/category.  
- If the category cannot be retrieved, it displays a “no game found” message.

## Example
`!game`  
→ `The current stream game is: Just Chatting`

If no category is available:  
→ `The current stream game is: no game found!`

## Customization
Edit `finalMessageBase` or `noGame` to change how the output appears.

Made by **BrianTU**