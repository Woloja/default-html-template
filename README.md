[![Build Status](https://travis-ci.com/cf-digital-ukraine/default-html-template.svg?branch=master)](https://travis-ci.com/cf-digital-ukraine/default-html-template) [![Codacy Badge](https://api.codacy.com/project/badge/Grade/43d32cd89e5e42dabcef8c0ad6aeb5a7)](https://www.codacy.com/app/cf-digital-ukraine/default-html-template?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=cf-digital-ukraine/default-html-template&amp;utm_campaign=Badge_Grade) [![Greenkeeper badge](https://badges.greenkeeper.io/cf-digital-ukraine/default-html-template.svg)](https://greenkeeper.io/) [![devDependency Status](https://david-dm.org/cf-digital-ukraine/default-html-template/dev-status.svg)](https://david-dm.org/cf-digital-ukraine/default-html-template#info=devDependencies) [![Dependency Status](https://david-dm.org/cf-digital-ukraine/default-html-template.svg)](https://david-dm.org/cf-digital-ukraine/default-html-template)
# Исходный шаблон для верстки
- Подробные зависимости можно посмотреть в [Пакет зависимостей](./package.json)  
- По умолчанию webpack prodaction собирает  
  - JavaScript совместимый с "ES6<" - браузерами  
  - postCss прогоняет вендоры - ```["last 2 versions", "ie >= 11", 'Firefox > 20', 'iOS > 8', 'Safari > 8']```  
  - postCss минимизирует и групирует медиа-запросы  

- По умолчанию webpack development делает тоже самое что и прод, за исключением компилирования babel, очистки и минификации кода  
  - postCss прогоняет вендоры - ```["last 1 versions"]```  

## INSTALL

Обязательно необходимо установить [Node.js with npm 6+](https://nodejs.org/uk/download/)
### Команды выполнять в терминале - корень package.json
<sup>Для загрузки всех development зависимостей </sup>
```shell
npm install
```
<sup>Для запуска слушателей файлов</sup>
```shell
npm run watch
```
  
Чтобы установить библиотеку, необходимо ее добавить в секцию dependencies файла [Пакет зависимостей](./package.json), после чего запустить `npm install`. Или выполнить команду `npm install *package-name* -S`
---
## Обязательная структура каталогов
<sup>Недостающие каталоги необходимо создать ручками</sup>
<pre>root
├── <a href="./resources/public" title="CF.Digital git">public</a>
│   ├── *.html
│   └── <a href="./resources/public/index.html" title="CF.Digital git">index.html</a>
├── <a href="./resources/resources" title="CF.Digital git">resources</a>
│   └── <a href="./resources/fonts" title="CF.Digital git">fonts</a>
│   │   └── bold  
│   │   │   ├── font-name.eot  
│   │   │   ├── font-name.svg  
│   │   │   ├── font-name.ttf  
│   │   │   ├── font-name.woff  
│   │   │   └── font-name.woff2  
│   │   ...
│   │   └── medium  
│   │       ├── font-name.eot  
│   │       ├── font-name.svg  
│   │       ├── font-name.ttf  
│   │       ├── font-name.woff  
│   │       └── font-name.woff2  
│   ├── <a href="./resources/image" title="CF.Digital git">image</a>
│   │   ├── folder  
│   │   │   ├── ...  
│   │   │   └── *.jpg|.svg|.png 
│   │   ├── ...  
│   │   └── *.jpg|.svg|.png 
│   ├── <a href="./resources/sass" title="CF.Digital git">sass</a>
│   │   ├── infoblock  
│   │   │   ├── ...
│   │   │   └── *.sass 
│   │   ├── pages  
│   │   │   ├── ...
│   │   │   └── *.sass  
│   │   ├── elements  
│   │   │   ├── ...
│   │   │   └── *.sass 
│   │   ├── <a href="./resources/sass/_default.sass" title="CF.Digital git">_default.sass</a>
│   │   ├── <a href="./resources/sass/_fonts.sass" title="CF.Digital git">_fonts.sass</a>
│   │   ├── <a href="./resources/sass/_functions.sass" title="CF.Digital git">_functions.sass</a>
│   │   ├── <a href="./resources/sass/_normalize.sass" title="CF.Digital git">_normalize.sass</a>
│   │   ├── <a href="./resources/sass/_variables.sass" title="CF.Digital git">_variables.sass</a>
│   │   ├── <a href="./resources/sass/app.sass" title="CF.Digital git">app.sass</a>
│   │   └── <a href="./resources/sass/old-ie.sass" title="CF.Digital git">old-ie.sass</a>
│   ├── <a href="./resources/js" title="CF.Digital git">js</a>
│   │   ├── ...custom-modules.js
│   │   ├── <a href="./resources/js/delta-functions.js" title="CF.Digital git">delta-functions.js</a>
│   │   └── <a href="./resources/js/app.js" title="CF.Digital git">app.js</a>
│   └── <a href="./resources/to-remove" title="CF.Digital git">to-remove</a>
│       ├── ...
│       └── ***.ext
├── <a href="./.gitignore" title="CF.Digital git">.gitignore</a>
├── <a href="./package.json" title="CF.Digital git">package.json</a>
├── <a href="./webpack.mix.js" title="CF.Digital git">webpack.mix.js</a>
└── <a href="./mix-manifest.json" title="CF.Digital git">mix-manifest.json</a>
</pre>
