# !dadjoke

A fun command that delivers a random dad joke pulled from an external API or JSON feed. The script reads the joke text, formats it with the user’s name, and sends it to chat. If no joke is available, the action quietly stops.

## Usage
`!dadjoke`

- The command replies directly to the user with a dad joke.  
- If the joke text is missing or empty, nothing is sent.

## Example
`!dadjoke`  
→ `@UserName, Why don't eggs tell jokes? They'd crack each other up.`

## Customization
Modify `messageTemplate` to change how the joke is displayed.  
You can also adjust the data source or parsing logic if you want different joke styles.

Made by **BrianTU**