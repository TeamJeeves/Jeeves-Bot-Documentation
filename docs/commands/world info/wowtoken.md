## WoWToken Command

### Description
The `wowtoken` command allows users to check the current price of the WoW Token in a specified region.

### Usage
```
/wowtoken [region]
```

### Options
- **region** (optional): Choose a different region. Default is `us`. Choices:
  - `us`: US/OC
  - `eu`: EU
  - `tw`: TW
  - `kr`: KR

### Permissions
- **User**: No special permissions required.
- **Bot**: No special permissions required.

### Examples
- Check the WoW Token price for the default region (US/OC):
  ```
  /wowtoken
  ```
- Check the WoW Token price for the EU region:
  ```
  /wowtoken region:eu
  ```

### Notes
- The command will display the current WoW Token price for the specified region.
- The bot will reply with an error message if it is unable to retrieve the token price data.

### Example:

![Wow Token Example](../../img/wowtoken.png)

*** 
