# telegram-arcade
A python, telegram game bot. The goal of this project is to make it simple to deploy games to a telegram bot. With this program, you can simply create an HTML5 game, add it to the config, register it with @botfather, and start playing your games!


# Installing and running

To run, create and fill out a `config.ini` file as follows
```
[DEFAULT]
API_KEY=<YOUR KEY HERE> 
GAMES = snake,stacker
HOST=127.0.0.1
PORT=9000
FEATURED=stacker
```

- `GAMES` is a comma seperated list of games to refer the user to. These should be include as an `html` file in the same directory (see `stacker.html` and `snake.html` as examples). You must also register each of these with @botfather as games with the same name.
- `HOST` and `PORT` should be the host and port that your games will be hosted on, which the telegram user will be refered to when they click to play your game.
- `FEATURED` will be the game that shows up when the user sends `/start`

Requires Python 3 and modules `python-telegram-bot` and `requests`. Run the bot with `python3 bot.py`.
