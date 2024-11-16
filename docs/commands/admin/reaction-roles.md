## Reaction Roles Command Documentation

### Overview
The `reaction-roles` command enables role assignments via reactions in Discord. This feature allows users to associate emojis with roles, making it easy to manage permissions and roles interactively within a specified channel.

---

### Key Features
- **Dynamic Role Assignment**: Assign roles when users click specific emojis.
- **Multi-Channel Support**: Use the same emoji for different roles in separate channels.
- **Customizability**: Supports all valid Discord emojis, including animated ones.
- **Permission Management**: Ensures proper role hierarchy and permissions for seamless operation.

---

### Usage Guide

#### 1. **Setup Listening Channel**
Run `/reaction-roles listen` to designate the channel where Jeeves will monitor for reaction events.  
**Syntax**:  
``` 
/reaction-roles listen channel:<#roles>
```  
**Notes**:
- Non-premium users can configure one listening channel.
- Premium users (via Patreon) can manage multiple listening channels.

---

#### 2. **Add Role Reactions**
Link an emoji to a role in the designated channel.  
**Syntax**:  
``` 
/reaction-roles add emoji:<emoji> role:<@Role> channel:<#channel> (optional for premium users)
```  
**Example**:  
```
/reaction-roles add emoji:💰 role:@GreedyGoblin
```

---

#### 3. **Remove Role Reactions**
Stop assigning a role linked to a specific emoji.  
**Syntax**:  
``` 
/reaction-roles remove emoji:<emoji> channel:<#channel> (optional for premium users)
```  
**Example**:  
```
/reaction-roles remove emoji:💰
```

---

#### 4. **View Role Reactions**
List all configured emojis and their associated roles in a server or specific channel.  
**Syntax**:  
```
/reaction-roles view
```

---

#### 5. **Clear All Reactions**
Remove all configured emojis and stop Jeeves from listening to any channels for Reaction Roles.  
**Syntax**:  
```
/reaction-roles clear
```  
⚠️ **Warning**: This action is irreversible and will reset all settings.

---

### Permissions
- **User Permissions**: `ManageRoles`
- **Bot Permissions**: `ManageRoles`  
Ensure Jeeves’ role is ranked higher than the roles it manages.

---

### Examples
- **Set Up a Role Reaction**:  
  ```
  /reaction-roles add emoji:🔔 role:@Subscriber channel:#roles
  ```
- **View All Reactions**:  
  ```
  /reaction-roles view
  ```

---

### FAQ

#### Q: How many RoleReactions can I have?  
**A**: Up to 50 per channel.

#### Q: Can I use the same emoji for different roles?  
**A**: Yes, but only in different channels.

#### Q: Can I have multiple emojis with the same name?  
**A**: No, Jeeves identifies emojis by their name, not by their icon or ID.

#### Q: How do I remove a deleted emoji from the configuration?  
**A**: Recreate the emoji with the same name, then use the `/reaction-roles remove` command.

---

### Notes
- Ensure Jeeves has the necessary permissions to manage roles.
- Premium users gain additional features, such as multiple role channels.

---
