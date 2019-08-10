# Visual Studio Code
## Настройка редактора Visual Studio Code

[Главная](https://damir-art.github.io)<br />
[Репозиторий](https://github.com/damir-art/visual-studio-code)

Visual Studio Code - на данный момент, один из самых популярных редакторов для HTML-верстальщиков и программистов. Аналог Sublime Text и Atom.

## Начальные настройки
* Шестеренка (снизу, слева) > Settings: автосохранение, размер шрифта
* Settings > User > Application > Telemetry: отключить
* Settings > Keyboard Shortcuts - посмотреть горячие ключи
* Settings > User Snippets - пользовательские сниппеты

## Плагины
**Live Server** - автообновление страниц браузера<br />
**Project Manager** - удобная работа с workspace<br />
**Beautify** - форматирование файлов HTML, CSS, JavaScript, JSON, Sass (ctrl+shift+p (F1), >beautify file)<br />
**Bracket Pair Colorizer** - делает код более удобочитаемым (подсветка скобок и т.д.)<br />
**Prettier - Code formatter** - автоматическое форматирование кода (Beautify?)<br />
**Javascript (ES6) Code Snippets** - сниппеты для ES6<br />
**Sass** - подсветка синтаксиса<br />
**Live Sass Compiler** - компиляция Sass/SCSS в CSS (автоматом устанавливает еще и Live Server)<br />
**Bootstrap 4, Font awesome 4, Font Awesome 5 Free & Pro snippets** - сниппеты + Awesome<br />
**Bootstrap v4 Snippets** - сниппеты и классы, ctrl + 'пробел' в любом свободном месте<br />
**Open in Browser** - открыть файл в браузере<br />
**npm** - удобная работа с npm<br />
**vscode-icons** - иконки в сайдбаре для ваших файлов<br />
**Better Comments** - подсветка комментариев кода<br />
**ESLint** - проверка правильности написания кода на JavaScript<br />
**Stylelint** - проверка правильности написания кода на CSS/SCSS/Sass/Less<br />
**GieLens** - раширение для более удобной работы с гит<br />
**Debugger for Chrome** - дебаггер для отладки JS-кода от гугл хром<br />
**Russian Language Pack for Visual Studio Code** - русификация

## Создание сниппета
* Settings > User Snippets > New Global Snippets File...
* Вводим имя файла, жмём Enter

Код сниппета:

    {
        "document.ready": {           // название сниппета
            "scope": "javascript",    // тип файла, в котором сработает сниппет
            "prefix": "doc",          // сокращённое название сниппета
            "body": [                 // код сниппета
                "jQuery(document).ready(function($ $1) {", 
                    "$0",
                "}); $2 "
            ],
            "description": "Полностью загруженный документ" // описание сниппета
        }
        // $число позиция курсора, перемещаемся по 'tab'
    }
    
## Горячие клавиши
`CTRL + P` - поиск по проекту<br />
`CTRL + SHIFT + P` - поиск по командам<br />
`ALT + SHIFT + F` - автоформатирование кода, встроенная функция VS Code

## Фишки
Если скопировал код, где табуляция два пробела, то жмешь alt + shift + f (становится 4, если столько указано в настройках).

### Интересные ссылки
https://habr.com/ru/company/ruvds/blog/460801/ - 27 плагинов<br />
https://www.youtube.com/watch?v=8qXIe7m8tLU&list=PLuY6eeDuleIMzp2sMA9NSj4UX_pI-jECS - миникурс
