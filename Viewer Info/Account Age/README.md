# !accountage / !accage

A utility command that reports the Twitch account age for you or another user. The script cleans the target name, retrieves the account age, formats it into readable time units, and sends the result to chat. It supports both self‑lookup and targeting another user, with an optional **full** mode for detailed output.

## Usage
`!accountage`  
`!accountage full`  
`!accountage <target>`  
`!accountage <target> full`  

`!accage` works identically.

- Without a target, the command reports **your** account age.  
- With a target, it reports **their** account age.  
- Adding **full** shows a detailed breakdown (years, months, weeks, days, hours, minutes, seconds).  
- Without **full**, the output is shortened to the first one or two time units.

## Example
`!accountage`  
→ `@UserName, you are 3 years & 2 months old.`

`!accage CoolStreamer full`  
→ `@UserName, @CoolStreamer is 2 years, 5 months, 1 week & 3 days old.`

## Customization
Edit `selfMessage` or `targetMessage` to change how results are displayed.  
Modify the `FormatTime` function to adjust time units or formatting rules.

Made by **BrianTU**