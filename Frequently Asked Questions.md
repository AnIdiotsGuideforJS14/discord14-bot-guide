Similar to the previous guide, this page has some FAQ's that people ask regarding JS14.
These are **generic examples** and will do **NOTHING** if you insert them into your code.
You must understand what they do.

In V14, there is a new enum called *ActivityType*, and can be used to set presence and status.

# Examples
```javascript
// This will set your bot as watching AnIdiotsGuide in Do-Not-Disturb
const { Client, GatewayIntentBits, ActivityType } = require('discord.js'); //import discord.js 

client.user.setPresence({
  activities: [{ name: `AnIdiotsGuide`, type: ActivityType.Watching }],
  status: 'dnd',
});
```