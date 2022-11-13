**📢 All about adding custom emojis to Discord Roles is here!**

⭐ _You can easily execute the steps with an eval command._

**Discord.js** actually has that functionality built-in with the **`GuildEmojiRoleManager`** class. The default collection is empty, making every emote accessible to every role. However, you can change that using the **`.add(), .remove(), and .set()`** methods.

### Here's how you can use it for your command;

First, get the emoji | **`message.guild.emojis.cache.get('<Emote ID>')`**

then the current role restrictions (default: none) | **`.roles`**

then add, set, or remove the specified role(s) | **`.add(['<Role ID>', '<Role ID>')`**

## Add emoji to role(s)
**`message.guild.emojis.cache.get('<Emote ID>').roles.add('<Role ID>')`**

## Set emoji from role(s)
**`message.guild.emojis.cache.get('<Emote ID>').roles.set('<Role ID>')`**

## Remove emoji to role(s)
**`message.guild.emojis.cache.get('<Emote ID>').roles.remove('<Role ID>')`**
