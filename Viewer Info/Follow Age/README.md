# !followage

A utility command that reports how long a user has been following the channel. The script cleans the target name, checks whether the user is following, formats the follow duration into readable time units, and sends the result to chat. It supports both self‑lookup and targeting another user, with an optional **full** mode for detailed output.

## Usage
`!followage`  
`!followage full`  
`!followage <target>`  
`!followage <target> full`

- Without a target, the command reports **your** follow age.  
- With a target, it reports **their** follow age.  
- Adding **full** shows a detailed breakdown (years, months, weeks, days, hours, minutes, seconds).  
- Without **full**, the output is shortened to the first one or two time units.  
- If the user is not following, the command returns a simple “not following” message.

## Example
`!followage`  
→ `@UserName, you have been following for 1 year & 3 months.`

`!followage CoolViewer full`  
→ `@UserName, @CoolViewer has been following for 2 years, 4 months, 2 weeks & 6 days.`

If not following:  
→ `@UserName, you are not following.`  
or  
→ `@UserName, @CoolViewer is not following.`

## Customization
Modify the follow‑related messages or adjust `FormatTime` to change time units or formatting rules.

Made by **BrianTU**