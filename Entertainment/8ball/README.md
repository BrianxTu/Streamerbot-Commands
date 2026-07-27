# !8ball

A fun command that gives a randomized Magic‑8‑Ball style response. The script selects a message from one of three categories—positive, neutral, or negative—and sends it to chat. Each response is fully randomized every time the command is used.

## Usage
`!8ball <question>`  
(or simply `!8ball`)

- The command replies directly to the user with a randomized 8‑ball answer.  
- The question itself is optional; the command will still respond even if no question is provided.

## Example
`!8ball Will I win my next game?`  
→ `@UserName, Outlook good.`

`!8ball`  
→ `@UserName, Reply hazy, try again.`

## Response Types
- **Positive** — confident yes‑style answers.  
- **Neutral** — vague or mysterious answers.  
- **Negative** — no‑style answers.

## Customization
Edit the positive, neutral, or negative arrays to change the tone or variety of responses.  
Modify `messageTemplate` to adjust how the final message is formatted.

Made by **BrianTU**