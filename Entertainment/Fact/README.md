# !fact

A simple fun command that delivers a random fact pulled from an external API or JSON feed. The script reads the fact text, formats it with the user’s name, and sends it to chat. If no fact is available, the action quietly stops.

## Usage
`!fact`

- The command replies directly to the user with a random fact.  
- If the fact text is missing or empty, nothing is sent.

## Example
`!fact`  
→ `@UserName, Honey never spoils — archaeologists have found edible honey in ancient tombs.`

## Customization
Modify `messageTemplate` to change how the fact is displayed.  
You can also adjust the data source or parsing logic if you want different types of facts.

Made by **BrianTU**