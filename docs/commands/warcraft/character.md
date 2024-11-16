## Characters Command Documentation

### Overview
The `characters` command allows users to manage their World of Warcraft characters linked to their Discord account through Jeeves. With this command, users can set a main character, view characters, update their information, and manage character visibility and ignore settings.

---

### Key Features
- **Set a Main Character**: Designate one character as your "main" for streamlined actions.
- **View Characters**: Display your characters or those of other users in the server.
- **Privacy Controls**: Hide or unhide specific characters from public visibility.
- **Management Tools**: Ignore or unignore characters to exclude them from all bot functions.

---

### Usage

#### General Command Syntax
```
/characters <subcommand> [options]
```

#### Subcommands and Usage

1. **Set-Main**
   - Designates one character as your main.
   - **Syntax**:  
     ```
     /characters set-main
     ```
   - Jeeves will prompt you with a dropdown list of your characters for selection.
   - Only one character can be set as your main at any time.

2. **View**
   - Displays a list of your characters or another user’s characters.
   - **Syntax**:  
     ```
     /characters view [user:@Username]
     ```
   - Without specifying a user, Jeeves displays your characters privately. If a user is specified, their characters are displayed publicly.

3. **Update**
   - Queues your characters for an update from the cache to reflect the latest changes (e.g., Raider.io score updates).
   - **Syntax**:  
     ```
     /characters update
     ```

4. **Hide and Unhide**
   - **Hide**: Marks a character as private, so others cannot see it.
     - **Syntax**:  
       ```
       /characters hide
       ```
   - **Unhide**: Makes a hidden character visible again.
     - **Syntax**:  
       ```
       /characters unhide
       ```
   - Jeeves will prompt you to select a character from your list for these actions.

5. **Ignore and Unignore**
   - **Ignore**: Excludes a character from all Jeeves systems, including role assignment and dropdown menus.
     - **Syntax**:  
       ```
       /characters ignore
       ```
   - **Unignore**: Reintegrates an ignored character into Jeeves systems.
     - **Syntax**:  
       ```
       /characters unignore
       ```
   - Jeeves will prompt you to select a character for these actions.

---

### Permissions
- **User Permissions**: No special permissions required.
- **Bot Permissions**: No special permissions required.

---

### Examples

- **Set a main character**:
  ```
  /characters set-main
  ```
- **View your characters**:
  ```
  /characters view
  ```
- **View another user's characters**:
  ```
  /characters view user:@Username
  ```
- **Update characters**:
  ```
  /characters update
  ```
- **Hide a character**:
  ```
  /characters hide
  ```
- **Ignore a character**:
  ```
  /characters ignore
  ```

---

### Notes
- Ensure you’ve linked your Battle.net account using the `/authorize` command before using the `characters` command.
- When setting a main character, hiding, unhiding, ignoring, or unignoring characters, Jeeves will provide a dropdown list for selection.
- Characters hidden or ignored will not appear in the `/characters view` list.

---

### FAQ

#### Q: Why can I only see 12 characters in `/characters view`?  
**A**: Due to Discord’s message length limit, Jeeves can only display up to 12 characters at a time. Rest assured, your other characters are still managed correctly.

#### Q: Can I ignore all characters?  
**A**: No, you must always have at least one character visible.

#### Q: Do I need to update characters manually often?  
**A**: Not typically. Updates are automatic for Jeeves Premium users, but the `/characters update` command can be used for immediate updates when needed.

---
