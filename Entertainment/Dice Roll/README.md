# !dice

A fun command that rolls one or more dice and reports the results. The script accepts an optional number, rolls that many dice (up to a maximum), and returns each individual roll.

## Usage
`!dice`  
`!dice <number>`  
`!roll <number>`  
`!rolldice <number>`  
`!diceroll <number>`

- Without a number, the command rolls **2 dice**.  
- With a number, it rolls up to the maximum allowed (default: 10).  
- Each die produces a random value between the configured minimum and maximum (default: 1–6).

## Example
`!dice`  
→ `@UserName, you rolled 2 dice and got 3, 6`

`!roll 5`  
→ `@UserName, you rolled 5 dice and got 2, 4, 1, 6, 3`

If the user enters an invalid number (non‑numeric or ≤ 0), the command defaults to rolling 2 dice.

## Customization
- Adjust `faceMin` and `faceMax` to change the dice range.  
- Modify `maxDiceAllowed` to increase or limit how many dice can be rolled.  
- Edit `messageTemplate` to change how results are displayed.

Made by **BrianTU**