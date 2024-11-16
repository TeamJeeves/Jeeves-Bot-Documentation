## Keystone Command Documentation

### Overview
The `keystone` command allows users to manage and view their Mythic+ keystones, making it easy to coordinate with guild members or server communities. Users can set their keystones, view shared keystones, share or unshare their keystone across servers, and manage live keystone boards.

---

### Key Features
- **Set Your Keystone**: Log your current Mythic+ dungeon keystone.
- **View Server Keystones**: See a list of all keystones shared on the server.
- **Share Across Servers**: Make your keystone visible in other Discord servers using Jeeves.
- **Manage Keystone Boards**: Install a live-updating board for premium users.

---

### Usage

#### General Command Syntax
```
/keystone <subcommand> [options]
```

#### Subcommands and Usage

1. **Set**
   - Log your current Mythic+ keystone, specifying dungeon and level.
   - **Syntax**:  
     ```
     /keystone set dungeon:<dungeon> level:<level> [character:<character>] [realm:<realm>]
     ```
   - **Required Parameters**:  
     - `dungeon`: The name of the dungeon.
     - `level`: The level of the keystone.  
   - **Optional Parameters**:  
     - `character`: The character that owns the keystone.
     - `realm`: The realm of the character.

   - **Example**:  
     ```
     /keystone set dungeon:the-necrotic-wake level:15 character:MyCharacter realm:MyRealm
     ```

---

2. **View**
   - Displays a list of keystones shared with the server.
   - **Syntax**:  
     ```
     /keystone view
     ```

   - **Example**:  
     ```
     /keystone view
     ```

---

3. **Share and Unshare**
   - **Share**: Make a keystone visible across multiple servers where Jeeves is active.
     - **Syntax**:  
       ```
       /keystone share character:<character> [realm:<realm>]
       ```
     - **Example**:  
       ```
       /keystone share character:MyCharacter realm:MyRealm
       ```

   - **Unshare**: Stop sharing a keystone with the server.
     - **Syntax**:  
       ```
       /keystone unshare character:<character> [realm:<realm>]
       ```
     - **Example**:  
       ```
       /keystone unshare character:MyCharacter realm:MyRealm
       ```

---

4. **Board**
   - Manage a live-updating keystone board for the server (premium feature).
   - **Subcommands**:  
     - `install`: Set up a keystone board.  
       ```
       /keystone board install
       ```
     - `uninstall`: Remove a keystone board.  
       ```
       /keystone board uninstall
       ```

---

### Permissions
- **User**: No special permissions required.
- **Bot**: No special permissions required.

---

### Notes
- Ensure you’ve linked your Battle.net account using the `/authorize` command before using the `keystone` command.
- When setting or sharing keystones, Jeeves will prompt you with dropdown options for ease of use.
- Keystone boards are available only for premium users (via Patreon).

---

### Examples
- Set a keystone:  
  ```
  /keystone set dungeon:the-necrotic-wake level:15 character:MyCharacter realm:MyRealm
  ```
- View server keystones:  
  ```
  /keystone view
  ```
- Share a keystone across servers:  
  ```
  /keystone share character:MyCharacter realm:MyRealm
  ```
- Install a live keystone board:  
  ```
  /keystone board install
  ```

---

### FAQ

#### Q: Can I share my keystone with multiple servers?  
**A**: Yes. Use `/keystone share` to make your keystone visible across all servers where Jeeves is active.

#### Q: What is the keystone board?  
**A**: A live-updating display of all keystones on the server. This feature is available to premium users.

#### Q: Can I set a keystone for a different character?  
**A**: Yes, use the optional `character` and `realm` parameters when setting or sharing a keystone.

---
