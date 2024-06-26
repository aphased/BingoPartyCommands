# BingoPartyCommands

You know why you're here:

## All available commands

Commands listed in the same line are aliases of one another, meaning they **achieve the same** thing equally, and exist to accommodate more users.

However, the one used in the primary column is how this feature is referred to in the documentation. Again, any will work, you can use whichever you prefer.

Features which work differently from Hypixel settings are explained.

|  Command    |                                                             Functionality                                                             |  Alias(es)      |
|-------------|---------------------------------------------------------------------------------------------------------------------------------------|-----------------|
| boopme      | `/boop`s you, the sender, back _if_ you have permissions. You can use this to test if everything is set up and that you are registered correctly.       |
| disband     | Is always disallowed.                                                                                                                 |                 |
| transfer    | Self-explanatory, should not need to be used though.                                                                                  |                 |
| mute        | Self-explanatory.                                                                                                                     | unmute          |
| promote     | Self-explanatory, but not even strictly required in this system. Leave IGN out to promote yourself.                                   | pro             |
| kickoffline | Self-explanatory, to make space for new players if party is full as Hypixel's limit is 100 players.                                   | kickafk, ko, ka |
| kick        | Self-explanatory.                                                                                                                     | remove          |
| block       | Kick/remove with additional ignore add.                                                                                               | ban             |
| unblock     | Revert ignore add, but don't re-invite.                                                                                               | unban           |
| stream      | (Re-)open party into a public one, with default size of 100, useful e.g. after briefly transferring to a non-MVP++ ranked player.     | public, open    |
| invite      | Self-explanatory. Leave IGN out to invite yourself.                                                                                   | inv             |
| allinvite   | Toggles the party setting.                                                                                                            |                 |
| speak       | Players with permissions can talk in party chat during p mute even without Hypixel party mod rank.                                    | say             |
| repeat      | Like speak, but with built-in repetitions of your message (2 seconds apart, maximum of 7). Defaults to 5 repetitions if the first word of your message isn’t a number. Don’t spam this. Useful e.g. for announcing a splash! | rep          |
| customrep   | Like repeat, but with more customization options. First argument is number of repetitions, second is waiting duration/pause between each message, then the rest is your text to be output. | customrepeat, crep, crepeat |
| rule        | Output Bingo Brewers' rules as listed in the Discord channel, 1-7. Defaults to saying rule 1 in party chat if no number was provided. |                 |
| guide       | Posts the link to this month's Bingo Guide by Indigo_Polecat on the [Hypixel Forums](https://hypixel.net). Sends only once per 30 seconds.    | gd, g           |
| poll        | Creates a Hypixel party poll. Don't spam this.                                                                                        |                 |
| help        | Points to the link for this readme.                                                                                                   |                 |


Developer/account-admin reserved (these won't work or make sense to use for anyone else):

|  Command       |                                                             Functionality               |  Alias(es)              |
|----------------|-----------------------------------------------------------------------------------------|-------------------------|
| cmd            | (Admin-only) executes any command if the sender is the bot account owner.               |                         |
| printAllowlist | Prints the currently used player data (who with which permissions) to console stdout.   | printallowed, lsallowed |
| setguide       | Override the Discord-fetched `!p guide` link and set it manually in case of failures.   | sg                      |


## Command alias

E.g. using Skytils mod (open config under `/st`, then `Edit Aliases`):
- Left side: `ap`
- Right side: `msg BingoParty !p`

… and you'll be able to `/ap mute`, `/ap kick spammerIGN`, etc. just like that!


## Implemented in

- [BingoPartyTools](https://github.com/aphased/BingoPartyTools)
- [BingoPartyBot](https://github.com/aphased/BingoPartyBot)


## License

BingoPartyCommands is open-sourced software and documentation licensed under the [MIT License](https://opensource.org/licenses/MIT).

