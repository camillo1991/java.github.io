[<img src="https://img.shields.io/badge/Telegram-%40Me-orange">](https://t.me/sho6ot)


![img1](.github/images/demo.png)

> 🇪🇳 README in english available [here](README-EN.md)

## Функционал  
| Функционал                                                     | Поддерживается  |
|----------------------------------------------------------------|:---------------:|
| Многопоточность                                                |        ✅        |
| Привязка прокси к сессии                                       |        ✅        |
| Авто-покупка предметов при наличии монет (tap, energy, charge) |        ✅        |
| Рандомное время сна между кликами                              |        ✅        |
| Рандомное количество кликов за запрос                          |        ✅        |
| Поддержка tdata / pyrogram .session / telethon .session        |        ✅        |


## [Настройки](https://github.com/shamhi/BlumCryptoBot/blob/main/.env-example)
| Настройка               | Описание                                                                  |
|-------------------------|---------------------------------------------------------------------------|
| **API_ID / API_HASH**   | Данные платформы, с которой запускать сессию Telegram _(сток - Android)_  |
| **CLAIM_RETRY**         | Количество попыток при неуспешном **Claim** _(напр. 3)_                   |
| **SLEEP_BETWEEN_CLAIM** | Задержка между **Claim** в минутах _(напр. 180)_                          |
| **SAVE_REFS_DATA**      | Сохранять ли реферальные данные _(True / False)_                          |
| **RANDOM_POINTS_COUNT** | Рандомное количество поинтов в игре _(напр. 50,150)_                      |
| **USE_PROXY_FROM_FILE** | Использовать-ли прокси из файла `bot/config/proxies.txt` _(True / False)_ |


## Установка
Вы можете скачать [**Репозиторий**](https://github.com/shamhi/BlumCryptoBot) клонированием на вашу систему и установкой необходимых зависимостей:
```shell
~ >>> git clone https://github.com/shamhi/BlumCryptoBot.git 
~ >>> cd BlumCryptoBot

# Если вы используете Telethon сессии, то клонируйте ветку "converter"
~ >>> git clone https://github.com/shamhi/BlumCryptoBot.git -b converter
~ >>> cd BlumCryptoBot

# Linux
~/BlumCryptoBot >>> python3 -m venv venv
~/BlumCryptoBot >>> source venv/bin/activate
~/BlumCryptoBot >>> pip3 install -r requirements.txt
~/BlumCryptoBot >>> cp .env-example .env
~/BlumCryptoBot >>> nano .env  # Здесь вы обязательно должны указать ваши API_ID и API_HASH , остальное берется по умолчанию
~/BlumCryptoBot >>> python3 main.py

# Windows
~/BlumCryptoBot >>> python -m venv venv
~/BlumCryptoBot >>> venv\Scripts\activate
~/BlumCryptoBot >>> pip install -r requirements.txt
~/BlumCryptoBot >>> copy .env-example .env
~/BlumCryptoBot >>> # Указываете ваши API_ID и API_HASH, остальное берется по умолчанию
~/BlumCryptoBot >>> python main.py
```

Также для быстрого запуска вы можете использовать аргументы, например:
```shell
~/BlumCryptoBot >>> python3 main.py --action (1/2)
# Или
~/BlumCryptoBot >>> python3 main.py -a (1/2)

# 1 - Создает сессию
# 2 - Запускает кликер
# 3 - Запуск через Telegram
```
