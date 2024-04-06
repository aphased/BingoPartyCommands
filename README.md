# BingoPartyCommands

You know why you're here:

## All available commands

Commands listed in the same line are aliases of one another, meaning they **achieve the same** thing equally, and exist to accommodate more users.

However, the one used in the primary column is how this feature is referred to in the documentation. Again, any will work, you can use whichever you prefer.

Features which work differently from Hypixel settings are explained.

|  Command    |                                                             Functionality                                                              |  Alias(es)   |
|-------------|----------------------------------------------------------------------------------------------------------------------------------------|--------------|
| disband     | Is always disallowed.                                                                                                                  |              |
| transfer    | Self-explanatory, should not need to be used though.                                                                                   |              |
| mute        | Self-explanatory.                                                                                                                      | unmute       |
| promote     | Self-explanatory, but not even strictly required in this system. Leave IGN out to promote yourself.                                    |              |
| kickoffline | Self-explanatory, to make space for new players if party is full as Hypixel's limit is 100 players.                                    | kickafk      |
| kick        | Self-explanatory.                                                                                                                      | remove       |
| block       | Kick/remove with additional ignore add.                                                                                                | ban          |
| unblock     | Revert ignore add, but don't re-invite.                                                                                                | unban        |
| stream      | (Re-)open party into a public one, with default size of 100, useful e.g. after briefly transferring to a non-MVP++ ranked player.      | public, open |
| invite      | Self-explanatory. Leave IGN out to invite yourself.                                                                                    | inv          |
| allinvite   | Toggles the party setting.                                                                                                             |              |
| speak       | Players with permissions can talk in party chat during p mute even without Hypixel party mod rank.                                     | say          |
| rule        | Output Bingo Brewers' rules as listed in the Discord channel, 1-7 (defaults to saying rule 1 in party chat if no number was provided). |              |
| poll        | Creates a Hypixel party poll. Don't spam this.                                                                                         |              |
| help        | Points to the link for this readme.                                                                                                    |              |
| cmd         | (Admin-only) executes any command if the sender is the bot account owner.                                                              |              |


## Command alias

E.g. using Skytils mod (open config under `/st`, then `Edit Aliases`):
- Left side: `ap`
- Right side: `msg BingoParty !p`

… and you'll be able to `/ap mute`, `/ap kick spammerIGN`, etc. just like that!


## Used in

- [BingoPartyTools](https://github.com/aphased/BingoPartyTools)
- [BingoPartyBot](https://github.com/aphased/BingoPartyBot)


## License

BingoPartyCommands is open-sourced software and documentation licensed under the [MIT License](https://opensource.org/licenses/MIT).

