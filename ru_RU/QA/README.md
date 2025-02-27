## Обновление LiteLoaderBDS
Скачайте новый `LiteLoader-версия.zip` из [Релиза](https://github.com/LiteLDev/LiteLoaderBDS/releases), распакуйте его в папку с BDS

## Как обновить Bedrock Dedicated Server (BDS)
Скачайте последнюю версию BDS с сайта [Minecraft.net](https://www.minecraft.net/en-us/download/server/bedrock), распакуйте все файлы, кроме `server.properties`,`allowlist.json`,`permission.json` to the old version of Bedrock Dedicated Server directory  
Затем запустите `LLPeEditor.exe` для генерации нового `bedrock_server_mod.exe`

## Как запустить LiteLoaderBDS на Linux
Мы не разработали версию для Linux систем, по этому вам нужно использовать [Wine](https://www.winehq.org/), чтобы запустить Windows Bedrock Dedicated Server (BDS), который требуется для работы LiteLoaderBDS, так же вы можете выбрать [докерный образ LiteLoader, или shell скрипт](https://github.com/LiteLDev/LiteLoaderBDS#for-linux) который мы сделали.

## Проблема утечек памяти на Wine
Это проблема Wine, мы не можем предоставить какое-либо решение, если вы используете контейнер Docker, вы можете ограничить память контейнера, чтобы предотвратить влияние утечки памяти.

## Поддержка LiteLoaderBDS новых версий Bedrock Dedicated Server
Минорные (хотфиксы и т.д.) версии BDS полностью совместимы.
Например: 2.1.2 разработана на основе BDS 1.18.11.01 и ее протокол 486. Пока версия протокола BDS (например: 1.18.12.01) будет 486, LL без проблем поддерживает ее.  
Версии где протокол не меняется мы называем минорными(например: 1.18.11.01 к 1.18.12.01), но если протокол измениться (как в 1.18.2 к 1.18.11.01), мы называем мажорным обновлением.
Версия игры и протокола будет показана при старте сервера, так же ее можно узнать через команду `version`.

## The compatibility of dll plugins
Тут так-же, как и с [Поддержкой LiteLoaderBDS новых версий Bedrock Dedicated Server](#Поддержка LiteLoaderBDS новых версий Bedrock Dedicated Server), некоторые плагины, которые имеют простые функции, которые чаще всего не трогают Mojang при обновлениях продолжают стабильно работать, а большие плагины, которые используют большой набор функций чаще всего перестают работать при обновлениях из-за смены функций.

## Совместимость скриптовых плагинов.
Если API LLScriptEngine не изменилось, скриптовые плагины(включая JavaScript и Lua) могут не обновляться для поддержки нового Bedrock Dedicated Server.

## Ошибки при загрузке плагинов.
- `126`  
Библиотека пропущена, проверьте правильность установки.

- `127`  
Плагин не совместим с текущей версией LiteLoaderBDS.

## Не могу запустить сервер через Wine
Попоробуйте удалить `plugins/LiteLoader/LLAutoUpdate.dll`  
Если память сервера меньше чем 1.2GB, добавьте памяти, LiteLoaderBDS требует больше памяти для запуска.

## Ошибки в логах
Загрузите соответствующую версию `PDB.zip` из [Релиза](https://github.com/LiteLDev/LiteLoaderBDS/releases), и распакуйте содержимое в следущие папки:
- `./`
- `./plugins/`
- `./plugins/lib`
