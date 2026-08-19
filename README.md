<div align="center">
<img align="center" width="200" height="200" src="https://raw.githubusercontent.com/VoidemLIVE/ProfileAssets/main/helpcommandTransparent.png" style="background-color:white;">

# HelpCommand Fork (Purpur 26.2)

Плагин **HelpCommand** от [VoidemLIVE](https://www.spigotmc.org/resources/help-command.102926/) — адаптированный форк под **Purpur 26.2**.

</div>

## Что это

Это форк оригинального плагина HelpCommand (v2.9.2), обновлённый для совместимости с серверами на базе **Purpur/Paper 26.2**. Оригинальный плагин поддерживал Spigot 1.18–1.21 — этот форк добавляет поддержку новой платформы.

## Что изменено

| Было (оригинал) | Стало (форк) |
|---|---|
| `spigot-api 1.18.1-R0.1-SNAPSHOT` | `paper-api 26.2.build.112-stable` |
| Java 1.8 | Java 21 |
| maven-compiler-plugin 3.8.1 | maven-compiler-plugin 3.13.0 |
| maven-shade-plugin 3.2.4 | maven-shade-plugin 3.5.1 |

### Подробнее

- **Замена Spigot API на Paper API** — Paper API включает совместимость со Spigot API, поэтому весь функционал (BungeeCord чат, PlaceholderAPI и т.д.) продолжает работать без изменений.
- **Java 21** — Required для Purpur 26.2.
- **Обновление Maven плагинов** — более новые версии корректно работают с Java 21.

## Сборка

```bash
git clone https://github.com/Zondermainy/Help-Command-Plugin.git
cd Help-Command-Plugin
mvn clean package
```

JAR будет в `target/HelpCommand-*.jar`.

## Установка

1. Скачай готовый JAR из [Releases](https://github.com/Zondermainy/Help-Command-Plugin/releases) или собери сам.
2. Положи в папку `plugins/`.
3. Перезапусти сервер.
4. Настрой файл `plugins/HelpCommand/config.yml` под свой сервер.

## Команды

| Команда | Описание |
|---|---|
| `/help [страница]` | Показать справку |
| `/hc reload` | Перезагрузить конфиг |
| `/hc sethelp` | Установить текущий HelpCommand (admin) |

## Оригинальный плагин

- [SpigotMC](https://www.spigotmc.org/resources/help-command.102926/)
- [GitHub (оригинал)](https://github.com/VoidemLIVE/Help-Command-Plugin)
- [Документация](https://hcdocs.voidem.com/)

## License

[MIT](https://choosealicense.com/licenses/mit/)
