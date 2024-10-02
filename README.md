# BingoPartyCommands

You know why you're here:

## All available commands

Commands listed in the same line are aliases of one another, meaning they **achieve the same** thing equally, and exist to accommodate more users.

However, the one used in the primary column is how this feature is referred to in the documentation. Again, any will work, you can use whichever you prefer.

Features which work differently from Hypixel settings are explained.

### Commands for anyone

- In-game on hypixel.net, you may `/boop BingoParty` (aka the public party leader account) in order to receive a `party invite`.
- You may request a link to this month's Bingo guide by sending `/pc !guide`. Don't spam this (the command also has a cooldown, and can be easily toggled off on the fly).

### Commands for all Bingo Brewers splashers & party moderators

|  Command    |                                                             Functionality                                                             |  Alias(es)      |
|-------------|---------------------------------------------------------------------------------------------------------------------------------------|-----------------|
| help        | Points to the link for this readme.                                                                                                   |                 |
| test        | See if YOU are on the permission list, and what permissions you have.  | boopme |

| disband     | Is always disallowed.                                                                                                                 |                 |
| transfer    | Self-explanatory, does not need to be used though. A receiving IGN has to be specified for this command (unlike with `promote`).      |                 |
| mute        | Self-explanatory.                                                                                                                     | unmute          |
| promote     | Self-explanatory, but not even strictly required in this system. Leave IGN out to promote yourself.                                   | pro, prom, promo |
| kickoffline | Self-explanatory, to make space for new players if party is full as Hypixel's limit is 100 players.                                   | kickafk, ko, ka |
| kick        | Self-explanatory.                                                                                                                     | remove          |
| ban         | Kick/remove with additional block (ignore) add.                                                                                       | block           |
| unban       | Revert block (ignore) add, but don't re-invite.                                                                                       | unblock         |
| stream      | (Re-)open party into a public one, with default size of 100, useful e.g. after briefly transferring to a non-MVP++ ranked player.     | public, open    |
| invite      | Self-explanatory. Leave IGN out to invite yourself.                                                                                   | inv             |
| allinvite   | Toggles the party setting.                                                                                                            | allinv, ai | 
| say         | Players with permissions can talk in party chat during p mute even without Hypixel party mod rank. (and even while not being in the party!) | speak           |
| repeat      | Like speak, but with built-in repetitions of your message (2 seconds apart, maximum of 7). Defaults to 5 repetitions if the first word of your message isn’t a number. Don’t spam this. Useful e.g. for announcing a splash! | rep          |
| customrepeat | Like repeat, but with more customization options. First argument is number of repetitions, second is waiting duration/pause between each message, then the rest is your text to be output. | customrep, crep, crepeat |
| rule        | Output Bingo Brewers' rules as listed in the Discord channel, 1-7. Defaults to saying rule 1 in party chat if no number was provided. |                 |
| guide       | Posts the link to this month's Bingo Guide by Indigo_Polecat on the [Hypixel Forums](https://hypixel.net). Sends only once per 30 seconds.    | gd, g           |
| poll        | Creates a Hypixel party poll. Don't spam this.                                                                                        |                 |

### Admin commands

Developer/account-admin reserved – these are set to not work for anyone else (due to not making sense to use, or offering too much access):

|  Command       |                                                             Functionality               |  Alias(es)              |
|----------------|-----------------------------------------------------------------------------------------|-------------------------|
| cmd            | (Admin-only) executes any command if the sender is the bot account owner.               |                         |
| limbo          | Sends the bot to Limbo | sendlimbo |
| addUser        | Adds users to the permission list |                 |
| removeUser     | Removes a user from the permission list |                 |
| getUser     | See if a user is on the permission list, and what permissions they have | query           |
| preferredName     | Sets your preferred name so the bot knows what to call you | pn              |

| close          | The reverse operation to `!p stream`.                                                   |                         |

| disable        | Temporarily toggle features/commands (e.g. `!p disable promote`).                       |                         |
| enable         | Undo the above (e.g. `!p enable promote`).                                              |                         |
| enableall      | Re-enable all currently temporarily disabled commands at once.                          |                         |

| reload          | Reloads all modifications to commands | load |

### Sudo commands

These commands should use the `!sudo` prefix.

|  Command       |                                                             Functionality               |  Alias(es)              |
|----------------|-----------------------------------------------------------------------------------------|-------------------------|
| drain        | Empties the party after a 10 second delay | empty           |

### Not implemented since rewrite

|  Command    |                                                             Functionality                                                             |  Alias(es)      |
|-------------|---------------------------------------------------------------------------------------------------------------------------------------|-----------------|
| printAllowlist | Prints the currently used player data (who with which permissions) to console stdout.   | printallowed, lsallowed |
| setguide       | Override the Discord-fetched `!p guide` link and set it manually in case of failures.   | sg                      |
| printDisabled  | List all of the currently deactivated/disabled commands to the console.                 | printdisabled, lsdisabled, lstoggled |

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

