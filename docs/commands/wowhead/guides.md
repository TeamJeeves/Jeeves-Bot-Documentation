## Guide Command

### Description
The `guide` command allows users to search Wowhead for guides related to World of Warcraft.

### Usage
```
/guide <search>
```

### Options
- **search** (required): The search term for the guide you want to find.

### Permissions
- **User**: No special permissions required.
- **Bot**: `EmbedLinks`

### Examples
- Search for a guide on Wowhead:
  ```
  /guide search:Mythic+ Dungeon Guide
  ```

### Notes
- Ensure that Jeeves has the necessary permission to send embedded messages.
- The bot will reply with an error message if it is unable to fetch guides or if no guides are found.
- The command will display the best matching guide from Wowhead, including an embedded message with details and a thumbnail if available.