# TerminalBot

A Telegram Bot based on [Pyrogram](https://github.com/pyrogram/pyrogram)

## installing

#### The Easy Way
[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/hackelite01/TerminalBot/)

#### The Legacy Way
Simply clone the repository and run the main file:

```sh
git clone https://github.com/hackelite01/TerminalBot.git
cd TerminalBot
virtualenv -p /usr/bin/python3 venv
. ./venv/bin/activate
pip install -r requirements.txt
# <Create config.py with variables as given below>
python3 -m termbot
```


## Getting config.py values

An example `config.py` file could be:

**Not All of the variables are mandatory**

__The Bot should work by setting only these variables__

```python3
from termbot.sample_config import Config

class Development(Config):
  APP_ID = 6
  API_HASH = "eb06d4abfb49dc3eeb1aeb98ae0f581e"
  TG_BOT_TOKEN = "123456789:eb98ae0f7-Gm_6d4abfb49dc_9dc3eBaEBa"
  AUTH_USERS = [
    997887920
  ]
```


## [Mayank](https://telegram.dog/mayank1rajput)

- Only four of the configuration / environment variables are mandatory.
- This is because of `pyrogram.errors.API_ID_PUBLISHED_FLOOD`
    - `APP_ID`:   You can get this value from https://my.telegram.org
    - `API_HASH`:   You can get this value from https://my.telegram.org
    - `TG_BOT_TOKEN`: You can create a bot using [@BotFather](https://telegram.dog/BotFather)
    - `AUTH_USERS`: space sperated IDs of users who are allowed to use the bot
    - `TG_UPDATE_WORKERS_COUNT`: Number of workers to use. `1` is the recommended amount see for yourself what works best!
- The bot should work without setting the non-mandatory environment variables.
- Please report any issues to the support group: [HackElite](https://t.me/hackelite01)

