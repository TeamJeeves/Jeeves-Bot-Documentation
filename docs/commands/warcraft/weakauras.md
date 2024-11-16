## Weakaura Command

### Description
The `weakaura` command allows users to search for Weakauras on Wago.IO and display the results.

### Usage
```
/weakaura <search>
```

### Options
- **search** (required): The search term for the Weakaura you want to find.

### Permissions
- **User**: No special permissions required.
- **Bot**: `EmbedLinks`

### Examples
- Search for a Weakaura:
  ```
  /weakaura search:Healing
  ```

### Notes
- Ensure that Jeeves has the necessary permission to send embedded messages.
- The bot will reply with an error message if there is an issue fetching information from Wago.IO or if no results are found.
- The command will display the first result from the search, including the Weakaura's name, description, views, favorites, and a link to the source on Wago.IO.