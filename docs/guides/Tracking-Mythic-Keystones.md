# Jeeves Discord Bot: Tracking Mythic Keystones

Enhance your server or guild's experience by utilizing Jeeves to efficiently track and manage Mythic Keystones. Here's a comprehensive guide:

## Manual Keystone Management

### Adding/Updating a Keystone:

Users can employ the following command to manually set or update a keystone:

```
/keystone set [dungeon] [key level]
```

**Note**: By default, Jeeves assumes you're referring to your primary character.

### For Players with Multiple Characters:

If you operate several characters and wish to specify a keystone for a non-main character, provide your character's name in the optional character parameter.

**Shorthand Naming**: Jeeves supports shorthand for character names. For instance, if your character's name is `DastardlyLock`, simply use a portion like `dast`, and Jeeves will discern the character for you.

## Automatic Keystone Tracking

For seamless and automatic keystone tracking:

1. **Download the Jeeves Desktop Client**: This client facilitates the auto-tracking of keystones. Check out the Client Download page for detailed information.
2. **Remember**: The Desktop Client updates data exclusively when you log in, log out, or reload the game.

## Viewing Keystones

To survey the available keystones, use the following command:

```
/keystone view
```

**For Premium Servers**: Premium servers possess an added feature—the Keystone Board. This board is essentially a dedicated channel showcasing a perpetually updated pinned message that displays available keystones.

## Important Information

- **Character Recognition**: It's crucial to know that Jeeves only identifies characters present during the authorization. Any alterations to the name or realm of a character, or the introduction of new characters, mandates re-authorization for accurate tracking.
