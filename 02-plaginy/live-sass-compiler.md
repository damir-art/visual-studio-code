# Live Sass Compiler
**Live Sass Compiler** - компиляция Sass/SCSS в CSS (автоматом устанавливает еще и Live Server)

- устанавливаем плагин
- создаём папку `scss`, в ней создаём файл `style.scss`, открываем
- внизу должно появиться `Watch Sass` и `Go Live`
- пишем код в файл
- жмём по `Watch Sass`, запустится наблюдатель, создастся файл .css в той же папке где находится .scss
- при изменении и сохранении кода в файле scss, файл css тоже будет обновляться

Настраиваем папку сохранения:
- нажимаем `shift + ctrl + p`
- Open Settings (JSON)

Добавляем туда код:

    "liveSassCompile.settings.generateMap": false,
    "liveSassCompile.settings.formats": [
        // This is Default.
        {
            "format": "expanded",
            "extensionName": ".css",
            "savePath": "/css"
        },
        // You can add more
        {
            "format": "compressed",
            "extensionName": ".min.css",
            "savePath": "/css"
        }
    ],
    "liveSassCompile.settings.autoprefix": [
        "> 1%",
        "last 2 versions"
    ]

## Разное
- SCSS IntelliSense - автодополнение
- SCSS Formatter - форматирование
