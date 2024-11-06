---
title: 'Функциональность'
date: 2024-11-06T11:18:33+05:00
description: Богатый и мощный набор функций Hugo обеспечивает основу и инструменты для создания статических сайтов, создаваемых за несколько секунд, а зачастую и меньше.
categories: [about]
keywords: []
menu:
  docs:
    parent: about
    weight: 30
weight: 30
toc: true
---
## Фреймворк

[Мультиплатформенность]
: Установите единственный исполняемый файл Hugo на Linux, macOS, Windows и другие платформы.

[Мультиязычность]
: Локализуйте проект для каждого языка и региона, включая переводы, изображения, даты, валюты, числа, проценты и последовательность символов. Мультиязычный фреймворк Hugo поддерживает однохостовые и многохостовые конфигурации.

[Форматы вывода]
: Верните каждую страницу вашего сайта в один или несколько выходных форматов, с возможностью детального контроля по типу страницы, разделу и пути. Хотя по умолчанию используется формат HTML, вы можете добавить JSON, RSS, CSV и другие. Например, создайте REST API для доступа к содержимому.

[Шаблоны]
: Создавайте шаблоны с помощью переменных, функций и методов для преобразования содержимого, ресурсов и данных в опубликованную страницу. Хотя шаблоны HTML являются наиболее распространенными, вы можете создавать шаблоны для любого формата вывода.

[Темы]
: Сократите время и стоимость разработки, используя одну из сотен тем, созданных сообществом Hugo. Темы доступны для корпоративных сайтов, проектов документации, портфолио изображений, целевых страниц, личных и профессиональных блогов, резюме, автобиографий и многого другого.

[Модули]
: Сократите время и стоимость разработки за счет создания или импорта упакованных комбинаций архетипов, активов, контента, данных, шаблонов, таблиц перевода, статических файлов или параметров конфигурации. Модуль может служить основой для нового сайта или дополнять существующий.

[Приватность]
: Настройте поведение встроенных шаблонов и шорткодов Hugo, чтобы обеспечить соответствие региональным нормам конфиденциальности, включая [GDPR] и [CCPA].

[Безопасность]
: Модель безопасности Hugo основана на том, что авторам шаблонов и конфигураций доверяют, а авторам контента - нет. Эта модель позволяет генерировать HTML-вывод, защищенный от внедрения кода. Другие средства защиты предотвращают «пересылку» в произвольные приложения, ограничивают доступ к определенным переменным окружения, предотвращают соединения с произвольными удаленными источниками данных и многое другое.

## Создание контента

[Форматы контента]
: Create your content using Markdown, HTML, AsciiDoc, Emacs Org Mode, Pandoc, or reStructuredText. Markdown is the default content format, conforming to the [CommonMark] and [GitHub Flavored Markdown] specifications.

[Атрибуты Markdown]
: Apply HTML attributes such as `class` and `id` to Markdown images and block elements including blockquotes, fenced code blocks, headings, horizontal rules, lists, paragraphs, and tables.

[Расширения Markdown]
: Leverage the embedded Markdown extensions to create tables, definition lists, footnotes, task lists, inserted text, mark text, subscripts, superscripts, and more.

[Хуки для рендеринга Markdown]
: Override the conversion of Markdown to HTML when rendering blockquotes, fenced code blocks, headings, images, links, and tables. For example, render every standalone image as an HTML `figure` element.

[Схемы]
: Use fenced code blocks and Markdown render hooks to include diagrams in your content.

[Математика]
: Include mathematical equations and expressions in Markdown using LaTeX or TeX typesetting syntax.

[Подсветка синтаксиса]
: Syntactically highlight code examples using Hugo's embedded syntax highlighter, enabled by default for fenced code blocks in Markdown. The syntax highlighter supports hundreds of code languages and dozens of styles.

[Шорткоды]
: Используйте встроенные шорткоды Hugo или создавайте свои собственные для вставки сложного контента. Например, с помощью шорткодов можно включать элементы `аудио` и `видео`, выводить таблицы из локальных или удаленных источников данных, вставлять фрагменты с других страниц и многое другое.

## Управление контентом

[Адаптеры контента]
: Create content adapters to dynamically add content when building your site. For example, use a content adapter to create pages from a remote data source such as JSON, TOML, YAML, or XML.

[Таксономия]
: Классифицируйте содержимое для установки простых или сложных логических связей между страницами. Например, создайте таксономию авторов и назначьте одного или нескольких авторов для каждой страницы. Помимо прочего, система таксономии обеспечивает инвертированный, взвешенный индекс для вывода списка связанных страниц, упорядоченных по релевантности.

[Данные]
: Augment your content using local or remote data sources including CSV, JSON, TOML, YAML, and XML. For example, create a shortcode to render an HTML table from a remote CSV file.

[Меню]
: Provide rapid access to content via Hugo's menu system, configured automatically, globally, or on a page-by-page basis. The menu system is a key component of Hugo's multilingual architecture.

[Управление URL]
: Serve any page from any path via global configuration or on a page-by-page basis.

## Конвейеры активов

[Обработка изображений]
: Convert, resize, crop, rotate,  adjust colors, apply filters, overlay text and images, and extract EXIF data.

[Комплектация JavaScript]
: Transpile TypeScript and JSX to JavaScript, bundle, tree shake, minify, create source maps, and perform SRI hashing.

[Обработка Sass]
: Transpile Sass to CSS, bundle, tree shake, minify, create source maps, perform SRI hashing, and integrate with PostCSS.

[Обработка Tailwind CSS]
: Compile Tailwind CSS utility classes into standard CSS, bundle, tree shake, optimize, minify, perform SRI hashing, and integrate with PostCSS.

## Производительность

[Кэширование]
: Сократите время и затраты на создание сайта за счет однократного рендеринга частичного шаблона и последующего кэширования результата, глобального или в определенном контексте. Например, кэшируйте результат конвейера активов, чтобы избежать повторной обработки на каждой отрисованной странице.

[Сегментация]
: Сократите время и затраты на создание сайта, разбив свои сайты на сегменты. Например, главная страница и «новостной раздел» рендерятся каждый час, а весь сайт - раз в неделю.

[Минификация]
: Минифицируйте HTML, CSS и JavaScript чтобы уменьшить размер файла, пропускную способность и время загрузки.

[CCPA]: https://en.wikipedia.org/wiki/California_Consumer_Privacy_Act
[Обработка Sass]: /functions/css/Sass/
[Caching]: /functions/partials/includecached/
[CommonMark]: https://spec.commonmark.org/current/
[Content adapters]: /content-management/content-adapters/
[Content formats]: /content-management/formats/
[Data]: /content-management/data-sources/
[Diagrams]: /content-management/diagrams/
[GDPR]: https://en.wikipedia.org/wiki/General_Data_Protection_Regulation
[GitHub Flavored Markdown]: https://github.github.com/gfm/
[Image processing]: /content-management/image-processing/
[JavaScript bundling]: /functions/js/build/
[Markdown attributes]: /content-management/markdown-attributes/
[Markdown extensions]: /getting-started/configuration-markup/#goldmark-extensions
[Markdown render hooks]: /render-hooks/introduction/
[Mathematics]: /content-management/mathematics/
[Меню]: /content-management/menus/
[Minification]: /getting-started/configuration/#configure-minify
[Модули]: https://gohugo.io/hugo-modules/
[Multilingual]: /content-management/multilingual/
[Multiplatform]: /installation/
[Output formats]: /templates/output-formats/
[Privacy]: /about/privacy/
[Security]: /about/security/
[Segmentation]: /getting-started/configuration/#configure-segments
[Shortcodes]: /content-management/shortcodes/
[Syntax highlighting]: /content-management/syntax-highlighting/
[Tailwind CSS processing]: /functions/css/tailwindcss/
[Taxonomies]: /content-management/taxonomies/
[Templates]: templates/introduction/
[Темы]: https://themes.gohugo.io/
[URL management]: /content-management/urls/