## Вёрстка макета "Charger"

[Ссылка на макет](https://cloud.mail.ru/public/FZMw/GhXkhN2oL)

## Работа с Gulp

## Установка и работа с шаблоном:

-   `npm install`
-   `gulp`

Шаблон начнет работать в режиме разработчика, без сжатия картинок и кода.

## Сборка

-   `gulp build`

Выполнится оптимизация кода и картинок.
После завершения действий галпом, папка с результатом готова к выгрузке на сервер/передаче заказчику

Внимание!
После выполнения `gulp build` создаются webp файлы картинок. Также они интегрируются в html и css.
Следовательно, стоит проверить все ли корректно отображается и работает.
Если после выполнения `gulp build` файлы редактировались, действие (`gulp build`) нужно повторить.

## Возможные проблемы и их решения:

### Ошибка node-sass.

Решения:

`npm rebuild node-sass`
и/или
`npm install sass gulp-sass --save-dev`

### Ошибка Pyton

Решениe:

`npm install --global windows-build-tools`

### Ошибка imagemin

Варианты решения :

-   папки и файлы должны быть названы латиницей без пробелов
-   тег img и его содержимое должны быть записаны в одну строку без переносов
-   в атрибуте src должен быть указан путь к существующей картинке
