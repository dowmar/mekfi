
## Functionality
| Functional                                                     | Supported |
|----------------------------------------------------------------|:---------:|
| Multithreading                                                 |     ✅     |
| Binding a proxy to a session                                   |     ✅     |
| Auto-purchase of items if you have coins (tap, energy, charge) |     ✅     |
| Random sleep time between clicks                               |     ✅     |
| Random number of clicks per request                            |     ✅     |
| Support tdata / pyrogram .session / telethon .session          |     ✅     |

## Settings
| Env                | Desc                                                                               |
|--------------------------|----------------------------------------------------------------------------------------|
| **API_ID / API_HASH**    | How to get ? (https://www.youtube.com/watch?v=JqJz2onGXQ4)           |
| **MIN_AVAILABLE_ENERGY** | Minimum amount of energy, it will delay after |
| **SLEEP_BY_MIN_ENERGY**  | Delay when reaching minimum energy in seconds (200)                                 |
| **ADD_TAPS_ON_TURBO**    | How many taps will be added when turbo is activated (2500)                          |
| **AUTO_UPGRADE_TAP**     | Should I improve the tap (True / False)                                                |
| **MAX_TAP_LEVEL**        | Maximum level of tap pumping example : (5)                                                    |
| **AUTO_UPGRADE_ENERGY**  | Should I improve the tap (True / False)                                                |
| **MAX_ENERGY_LEVEL**     | Maximum level of tap pumping (eg 5)                                                    |
| **AUTO_UPGRADE_CHARGE**  | Should I improve the tap (True / False)                                                |
| **MAX_CHARGE_LEVEL**     | Maximum level of tap pumping (eg 5)                                                    |
| **APPLY_DAILY_ENERGY**   | Whether to use the daily free energy boost (True / False)                              |
| **APPLY_DAILY_TURBO**    | Whether to use the daily free turbo boost (True / False)                               |
| **RANDOM_CLICKS_COUNT**  | Random number of taps ([50,200])                                                      |
| **SLEEP_BETWEEN_TAP**    | Random delay between taps in seconds ([10,25])                                        |
| **USE_PROXY_FROM_FILE**  | (False)            |

## Installation
```shell
~ >>> git clone https://github.com/dowmar/mekfi.git
~ >>> cd mekfi

#Linux
~/mekfi >>> python3 -m venv venv
~/mekfi >>> source venv/bin/activate
~/mekfi >>> pip3 install -r requirements.txt
~/mekfi >>> cp .env-example .env
~/mekfi >>> nano .env # Here you must specify your API_ID and API_HASH , the rest is taken by default
~/mekfi >>> python3 main.py

#Windows
~/mekfi >>> python -m venv venv
~/mekfi >>> venv\Scripts\activate
# If there is an error in powershell like "“Cannot be loaded because running scripts is disabled on this system”"
# use this
~/mekfi >>> powershell -ExecutionPolicy Bypass venv\Scripts\activate
# continue below
~/mekfi >>> pip install -r requirements.txt
~/mekfi >>> copy .env-example .env
~/mekfi >>> # Specify your API_ID and API_HASH, the rest is taken by default
~/mekfi >>> python main.py
```

Also for quick launch you can use arguments, for example:
```shell
~/mekfi >>> python3 main.py --action (1/2)
# Or
~/mekfi >>> python3 main.py -a (1/2)

#1 - Create session
#2 - Run clicker
```
