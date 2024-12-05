# Victini

A Discord bot written in Python using [Discord.py](https://github.com/Rapptz/discord.py)

Victini's primary function is to spin the [V-Wheel](https://bulbapedia.bulbagarden.net/wiki/Victini_(Gates_to_Infinity)) daily and hoist the relevant Pokémon type roles (Fire, Grass, Electric, etc.) in the server for 24 hours.

Secondary functions include some user-facing commands, invoked using the `!` prfix. The current list of available commands are as follows:

| Command | Effects                                 | Permissions |
|----------|-----------------------------------------|-------------|
| !pet     | Pets Victini (They might not like that) | Everyone    |


### Installation & Requirements

Currently, you must populate a `.env` file with two values:

- `DISCORD_TOKEN` must be populated with the bot's auth token from the developer portal
- `VWHEEL_CHANNEL_ID` must have the channel ID of the v-wheel channel

#### Required permissions

The bot must be granted the following role permissions in order to function correctly:
- `Manage Roles`

Additionally, the bot's role (Probably called `Victini`) _must_ be listed ABOVE all of the Pokémon Type roles in the list of roles in order to manipulate their hoisted status.

#### Server Settings

Your Discord server MUST have 18 "Type" roles available and they must have *exactly* the names as follows:

- Normal Type
- Fire Type
- Water Type
- Grass Type
- Electric Type
- Ice Type
- Fighting Type
- Poison Type
- Ground Type
- Flying Type
- Psychic Type
- Bug Type
- Rock Type
- Ghost Type
- Dragon Type
- Dark Type
- Steel Type
- Fairy Type

Once all of the above requirements are met, Victini should run as expected.