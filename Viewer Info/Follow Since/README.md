# !followsince

A utility command that reports the exact date a user began following the channel. The script cleans the target name, checks whether the user is following, calculates the follow date, formats it, and sends the result to chat. It supports both self‑lookup and targeting another user.

## Usage
`!followsince`  
`!followsince <target>`

- Without a target, the command reports **your** follow date.  
- With a target, it reports **their** follow date.  
- If the user is not following, the command returns a simple “not following” message.

## Example
`!followsince`  
→ `@UserName, you followed on 3/14/2021 8:22:10 PM.`

`!followsince CoolViewer`  
→ `@UserName, @CoolViewer followed on 6/2/2019 1:05:47 PM.`

If not following:  
→ `@UserName, you are not following.`  
or  
→ `@UserName, @CoolViewer is not following.`

## Customization
Edit `selfMessage`, `targetMessage` to change how results are displayed.
Edit `dateFormat` to change how the date is displayed.

Made by **BrianTU**