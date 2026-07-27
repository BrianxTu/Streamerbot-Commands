# !quote — README

A full quote system that supports adding quotes, removing quotes, retrieving quotes by ID, and pulling a random quote. Because of Streamer.bot Csharp logic in this particular case, the logic is split into two wired actions:  
**Action 1:** Interprets the user’s intent (add, remove, get, random). 
**Streamer.bot** Add's, removes, gets the quote/random. 
**Action 2:** Processes the result and sends the final message to chat.

## Usage
`!quote`  
`!quote <id>`  
`!quote add <text>`  
`!quote remove <id>`  
Aliases for remove: `remove`, `delete`, `del`

### Behavior
- **No arguments** → returns a **random quote**.  
- **Number** → returns the quote with that **ID**.  
- **add <text>** → adds a new quote (moderators only).  
- **remove <id>** → removes a quote (moderators only).

## Examples
`!quote`  
→ `@UserName, id:14 - 'Never trust a goose with a plan.'`

`!quote 7`  
→ `@UserName, id:7 - 'Chat demanded snacks.'`

`!quote add This stream is powered by caffeine.`  
→ `@UserName, quote 22 added.`

`!quote remove 5`  
→ `@UserName, quote 5 removed.`

If something fails:  
→ `@UserName, failed to process quote.`

## Customization
Edit the message templates in the second action to change how quotes are displayed, added, or removed.

Made by **BrianTU**