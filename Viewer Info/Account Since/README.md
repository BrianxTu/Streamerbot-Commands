# !accountsince / !accsince

A utility command that reports the exact date a Twitch account was created. The script cleans the target name, retrieves the account creation timestamp, formats it, and sends the result to chat. It supports both self‑lookup and targeting another user.

## Usage
`!accountsince`  
`!accountsince <target>`  

`!accsince` works identically.

- Without a target, the command reports **your** account creation date.  
- With a target, it reports **their** creation date.

## Example
`!accountsince`  
→ `@UserName, you created your account on 3/14/2020 8:22:10 PM.`

`!accsince CoolStreamer`  
→ `@UserName, @CoolStreamer created their account on 6/2/2018 1:05:47 PM.`

## Customization
Edit `selfMessage`, `targetMessage` to change how results are displayed.
Edit `dateFormat` to change how the date is displayed.

Made by **BrianTU**