# ThunkBot_Suggestions
Bug reports and suggestions for ThunkBot

## ThunkBot command documentation

[Available here](./Commands.md)

## Other functionality

* Automatically sets idle status after 15 minutes of no server activity. And then plays ominous video games.
* Keeps track of praise (either via `:heart:` reaction to commands or via `!goodbot`
* Keeps track of most used commands and who invoked the most commands.
* Can automatically respond to or add reactions to messages with certain keywords
   * For example: If you link to TVTropes, ThunkBot will post a warning about the dangers of that site.
   * If you are bothered by one of these reactions, ThunkBot has an exception list for each. 
* Notifies the owner (me) if shut down.

## Privacy

The Bot keeps track of the following data:

1) How many times each user invoked a command
2) How many times each command was invoked
3) How many times the bot was thanked (but not by whom)
4) The bot logs [exceptions](https://en.wikipedia.org/wiki/Exception_handling) that occur during event handling and command execution. I keep user related information out of these logs to the best of my ability.
   
Note: Number 1 and 2 are strictly separated. The bot does not keep track of how many times each user used a specific command.
