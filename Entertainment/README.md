# Entertainment Commands  
A set of simple, fun StreamerBot commands designed to add personality and interaction to your chat.

These commands are lightweight, easy to modify, and work across all platforms StreamerBot supports.

---

## Commands Included  
- 8ball  
- Coin Flip  
- Dad Joke  
- Dice Roll  
- Fact  
- Quote  

Each command supports multiple aliases, optional variables, and full customization through C#.

---

## 8ball  
A classic random-response command for quick chat interaction.

**Command:**  
`!8ball <message>`

**Description:**  
Returns a random magic 8ball-style answer. Works with or without a message.

---

## Coin Flip  
Simple and perfect for chat decisions.

**Commands:**  
`!coin`  
`!coinflip`  
`!flip`  
`!flipcoin`

**Description:**  
Returns either Heads or Tails.

---

## Dad Joke  
Because chat deserves pain.

**Command:**  
`!dadjoke`

**Description:**  
Returns a random dad joke.

---

## Dice Roll  
Roll one or multiple dice.

**Commands:**  
`!roll <amount>`  
`!rolldice <amount>`  
`!dice <amount>`  
`!diceroll <amount>`

**Description:**  
Rolls up to 10 dice at once (limit is configurable).  
If no number is provided, defaults to two die.

**Examples:**  
`!roll`  
`!roll 5`

---

## Fact  
Random trivia for chat engagement.

**Command:**  
`!fact`

**Description:**  
Returns a random fact from a customizable list.

---

## Quote  
Add, remove, or display quotes.

**Commands:**  
`!quote`  
`!quote <id>`  
`!quote add <message>`  
`!quote remove <id>`  
`!quote delete <id>`  
`!quote del <id>`

**Description:**  
- Using no arguments returns a random quote.  
- Using an ID returns the quote with that ID.  
- Using "add" followed by a message adds a new quote.  
- Using "remove", "delete", or "del" followed by an ID removes the quote.
