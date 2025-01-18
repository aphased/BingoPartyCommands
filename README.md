# BingoPartyCommands

Table of Contents:

- [Available commands](#available-commands)
  - [Public commands](#public-commands)
  - [Splasher commands](#splasher-commands)
  - [Staff commands](#staff-commands)
- [Additional tips](#additional-tips)
  - [Alias command](#alias-command)
  - [Discord account linking](#discord-account-linking)
  - [Alt accounts](#alt-accounts)
- [Implementations](#implemented-in)
- [License](#license)

## Available commands

Commands are executed by running `/msg BingoParty !p <command> <arguments>` in-game, or using the discord command in the bridge channel accessible to all BingoBrewers splashers after linking their accounts.

> [!TIP]
> If you are a BingoBrewers splasher or party moderator, instructions on how to link your Minecraft and Discord accounts can be found in the [`Additional tips`](#additional-tips) section.

Commands listed in the `Aliases` column are functionally equivalent to the one in the primary column, and exist to accommodate more users, as well as to provide shorter and more memorable alternatives.

The primary name is generally how the feature is referred to in the documentation, but you can use whichever you prefer.

> [!NOTE]
> Command usage instructions are noted with specific formatting. Example usage: `!p example <arg1> <arg2.1|arg2.2> [arg3]`
>
> - Literal strings are not surrounded by any brackets: `!p example`
> - Required arguments are wrapped in angle brackets: `<arg1>`
> - Multiple possible values are separated by a pipe symbol: `<arg2.1|arg2.2>`
> - Optional arguments are wrapped in square brackets: `[arg3]`

### Public commands

- In-game on Hypixel, you may `/boop BingoParty` in order to be invited to the party, as an alternative to `/p join BingoParty`.

<!--begin-section-public-commands-->

#### Miscellaneous commands

| Command | Functionality                                                                          | Aliases                                                 |
| ------- | -------------------------------------------------------------------------------------- | ------------------------------------------------------- |
| `test`  | Check whether you have party permissions and which permission rank you're assigned to. | `testpermissions`, `testperms`, `testcommand`, `boopme` |

#### Party commands

#### Public commands

These commands are publicly usable by sending them directly into the party chat. Use them by running `/pc <command>`.

| Command  | Functionality                                                           | Aliases |
| -------- | ----------------------------------------------------------------------- | ------- |
| `!guide` | Send a link to this month's bingo guide in party chat. (public command) | `!gd`   |

<!--end-section-public-commands-->

### Splasher commands

The following commands can be executed by all BingoBrewers splashers and party moderators.

<!--begin-section-splasher-commands-->

#### Administrative commands

| Command | Usage                 | Functionality                           | Aliases                |
| ------- | --------------------- | --------------------------------------- | ---------------------- |
| `query` | `!p query <username>` | Check another person's permission rank. | `getuser`, `queryuser` |

#### Miscellaneous commands

| Command         | Usage                                 | Functionality                                                                                                           | Aliases            |
| --------------- | ------------------------------------- | ----------------------------------------------------------------------------------------------------------------------- | ------------------ |
| `help`          | `!p help list` or `!p help <command>` | Get information about a specific command, including description, usage and aliases.                                     |                    |
| `hiderank`      | `!p hiderank [true\|false]`           | Toggle whether the bot should include your hypixel rank in message output.                                              | `hr`, `togglerank` |
| `link`          | `!p link <discord code>`              | Link your Discord and Minecraft accounts. See tips in the online documentation for more info.                           |                    |
| `preferredname` | `!p preferredname [alt username]`     | Mark one of your accounts as the main, "preferred" username. This will be the name used by the bot in certain commands. | `pn`, `name`       |

#### Party commands

The following commands allow interaction with the party and moderation thereof.

| Command       | Usage                                                                                               | Functionality                                                                      | Aliases                             |
| ------------- | --------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ----------------------------------- |
| `allinvite`   | `!p allinvite`                                                                                      | Toggle the ability for anyone to invite people.                                    | `allinv`, `ai`                      |
| `ban`         | `!p ban <username> [reason]`                                                                        | Kick and `/block add` a player to prevent them from rejoining.                     | `block`                             |
| `guide`       | `!p guide`                                                                                          | Send a link to this month's bingo guide in party chat.                             | `gd`, `g`                           |
| `invite`      | `!p invite [username]`                                                                              | Invite someone to the party. Defaults to yourself.                                 | `inv`                               |
| `kick`        | `!p kick <username>`                                                                                | Kick a player from the party.                                                      | `remove`                            |
| `kickoffline` | `!p kickoffline`                                                                                    | Kick all offline players from the party.                                           | `ko`, `kickafk`, `ka`               |
| `mute`        | `!p mute`                                                                                           | Mute/Unmute the party.                                                             | `unmute`                            |
| `open`        | `!p open [size]`                                                                                    | (Re-)Open the party up to the public (`/stream open`).                             | `public`, `stream`                  |
| `promote`     | `!p promote [username]`                                                                             | Promote a player to party moderator. Defaults to yourself.                         | `promo`, `prom`, `pro`              |
| `rule`        | `!p rule [number]`                                                                                  | Send a BingoBrewers rule in party chat.                                            |                                     |
| `transfer`    | `!p transfer <username>`                                                                            | Transfer the party to someone else. Avoid using this.                              |                                     |
| `unban`       | `!p unban <username>`                                                                               | Unblock a player (`/block remove`).                                                | `unblock`                           |
| `splash`      | `!p splash <hub number> [hub id]` or `!p splash /p join <username>` or `!p splash switch <new hub>` | Announce a splash in party chat. The bot will send the announcement several times. | `hub`, `announcesplash`, `announce` |
| `poll`        | `!p poll <spellbingo\|goalscompleted\|playtime\|splashwhen>`                                        | Start a poll from one of several available poll presets in party chat.             |                                     |

<!--end-section-splasher-commands-->

### Staff commands

The following commands are restricted due to the elevated access they provide. Depending on the function, they are each executable either only by the bot account owner or by users with BingoBrewers staff permissions.

<!--begin-section-staff-commands-->

#### Administrative commands

| Command        | Permission | Usage                                                                               | Functionality                                                                                                                  | Aliases                           |
| -------------- | ---------- | ----------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------ | --------------------------------- |
| `adduser`      | Staff      | `!p adduser <user> <(updated)permission>` or `!p adduser <new alt> <existing main>` | Add a new user or alt account to the permission database or modify an existing user's permission level.                        | `user`                            |
| `limbo`        | Staff      | `!p limbo`                                                                          | Manually send the bot to limbo. This shouldn't ever be necessary anymore.                                                      | `sendlimbo`                       |
| `removeuser`   | Staff      | `!p removeuser <username> [only]`                                                   | Remove a user or a single account from the permission database.                                                                |                                   |
| `disable`      | Admin      | `!p disable <command1> [command2]...` or `!p disable <all\|most>`                   | Disable bot commands from being used. Note that certain commands can't be disabled.                                            |                                   |
| `enable`       | Admin      | `!p enable <command1> [command2]...` or `!p enable <all\|some>`                     | Re-enable previously disabled commands.                                                                                        |                                   |
| `listdisabled` | Admin      | `!p listdisabled`                                                                   | List all currently disabled commands.                                                                                          | `disabled`, `lsdisabled`, `lsoff` |
| `setguide`     | Admin      | `!p setguide <link> [MM/YYYY]`                                                      | Manually set this month's bingo guide link. Usage is discouraged, configure a discord guide channel in the bot config instead. |                                   |
| `cmd`          | Owner      | `!p cmd <command>`                                                                  | Execute any command as the bot account.                                                                                        | `execute`, `exec`                 |
| `reload`       | Owner      | `!p reload`                                                                         | Reload all commands from their file.                                                                                           | `reloadcommands`, `load`          |
| `setverbosity` | Owner      | `!p setverbosity <verbosity level> [confirm]`                                       | Set the verbosity setting, which can reduce unnecessary chat output.                                                           | `verbosity`                       |
| `updatenames`  | Owner      | `!p updatenames [confirm]`                                                          | Manually trigger a refresh of all usernames from their UUID using Mojang's API. This is scheduled automatically.               | `refreshnames`                    |

#### Party commands

The following commands allow interaction with the party and moderation thereof.

| Command         | Permission | Usage                 | Functionality                                                | Aliases                     |
| --------------- | ---------- | --------------------- | ------------------------------------------------------------ | --------------------------- |
| `close`         | Staff      | `!p close [reason]`   | Close the party to the public (`/stream close`).             | `private`                   |
| `canceldisband` | Admin      | `!p canceldisband`    | Abort a party disband within the 10 second grace period.     | `cdisband`, `disbandcancel` |
| `canceldrain`   | Admin      | `!p canceldrain`      | Abort a party drain within the 10 second grace period.       | `cdrain`, `draincancel`     |
| `disband`       | Admin      | `!p disband [reason]` | Disband the party after a 10 second delay. Avoid using this. |                             |
| `drain`         | Admin      | `!p drain [reason]`   | Drain the party after a 10 second delay. Avoid using this.   | `empty`                     |

#### Unrestricted chat commands

The following commands provide a way to send arbitrary messages through the bot account, which is reserved to staff due to the risk of its usage getting the bot account punished.

| Command   | Permission | Usage                                                              | Functionality                                                                                               | Aliases                                    |
| --------- | ---------- | ------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------- | ------------------------------------------ |
| `flea`    | Staff      | `!p flea <message>`                                                | Repeat any message in party chat with predefined parameters. Restricted due to allowing arbitrary messages. | `bossflea`, `bf`                           |
| `rawpoll` | Staff      | `!p rawpoll <Question/Answer1/Answer2/Optional/Optional/Optional>` | Start a custom poll in party chat. Restricted due to allowing arbitrary messages.                           | `rpoll`                                    |
| `repeat`  | Staff      | `!p repeat [repetitions] [delay] <message>`                        | Repeat any message in party chat multiple times. Restricted due to allowing arbitrary messages.             | `rep`, `customrepeat`, `crep`, `customrep` |
| `say`     | Staff      | `!p say <message>`                                                 | Send any message in party chat through the bot. Restricted due to allowing arbitrary messages.              | `speak`                                    |

<!--end-section-staff-commands-->

## Additional tips

### Alias command

Setting up an alias command is recommended to reduce the length of the commands you need to type. This can be accomplished for example using the [Skytils mod](https://github.com/Skytils/SkytilsMod) (open the config under `/st`, then `Edit Aliases`):

Create a new alias and fill the fields as follows:

- **Left side (alias)**: `ap` (you can choose any alias you like, recommended ones are `ap` or `b`)
- **Right side (command to run)**: `msg BingoParty !p`

> [!NOTE]
> Notice both values are entered without a leading slash (`/`).

You can now use `/ap mute`, `/ap kick <spammerIGN>`, etc. with much less typing!

### Discord account linking

If you are a BingoBrewers splasher, you have the option to link your Discord account to your Minecraft account(s) for the ability to use BingoParty commands from Discord.
Follow these steps to link your accounts:

- Use the `/link` command available on Discord in the bridge channel (`#bingo-party-chat-logs`) to obtain a linking code, valid for 5 minutes.
- Run `/msg BingoParty !p link <code>` in-game with the previously obtained code from the account you wish to link.

If completed successfully, you'll now be able to interact with the bot through Discord using the `/run` command available in the bridge channels.

### Alt accounts

If you'd like to use BingoParty commands from your alt(s), for example if you have a dedicated splashing account, you can ask a bot administrator or any member of staff in BingoBrewers, who will be able to grant your account the appropriate permissions.

## Implemented in

- [BingoPartyBot](https://github.com/aphased/BingoPartyBot)
- [BingoPartyTools](https://github.com/aphased/BingoPartyTools) (currently outdated, missing most commands)

## License

BingoPartyCommands is open-sourced software and documentation licensed under the [MIT License](https://opensource.org/licenses/MIT).
