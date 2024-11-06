---
title: Меню
description:  Создайте меню, определив пункты, локализовав каждый из них и отобразив полученную структуру данных.
categories: [content management]
keywords: [menus]
menu:
  docs:
    parent: content-management
    weight: 190
weight: 190
toc: true
aliases: [/extras/menus/]
date: 2024-11-06T12:49:50+05:00
---

## Обзор

Чтобы создать меню для вашего сайта, выполните следующие действия:

1. Определите пункты меню
2. [Локализуйте] каждый пункт
3. Оформите меню в виде [шаблона]

Создайте несколько меню, плоских или вложенных. Например, создайте главное меню для верхнего колонтитула и отдельное меню для нижнего колонтитула.

Существует три способа определения пунктов меню:

1.  Автоматически
2.  На главной странице
3.  В конфигурации сайта

> Хотя вы можете использовать эти методы в комбинации при определении меню, меню будет проще концептуализировать и поддерживать, если вы будете использовать один метод для всего сайта.

## Автоматическое определение

Чтобы автоматически определить пункт меню для каждого верхнего уровня [раздела](https://gohugo.io/getting-started/glossary/#section) вашего сайта, включите меню страниц раздела в конфигурации сайта.     

```yaml
sectionPagesMenu: main
```

Это создает структуру меню, к которой вы можете обращаться с помощью `site.Menus.main` в ваших шаблонах. Подробности см. в разделе [Шаблоны меню].

## Определение на главной странице

Чтобы добавить страницу в "Главное" (main) меню:

```yaml
---
menus: main
title: About
---
```

Обратитесь к записи с помощью `site.Menus.main` в ваших шаблонах. Подробности см. в разделе [Шаблоны меню].

Чтобы добавить страницу в меню «главная» и «нижний колонтитул»:

content/contact.md
```yaml
---
menus:
- main
- footer
title: Contact
---
```

В ваших шаблонах доступ к этому пункту осуществляется с помощью `site.Menus.main` и `site.Menus.footer`. Подробности см. в разделе [Шаблоны меню].

В приведенных выше примерах ключом конфигурации является `menus`. Ключ конфигурации `menu` (единственное число) является псевдонимом для `menus`.

### Свойства {#properties-front-matter}

Используйте эти свойства при определении пунктов меню во фронтальном материале:

identifier
: (`string`) Требуется, когда два или более пункта меню имеют одинаковое `name`, или при локализации `name` с помощью таблиц перевода. Должно начинаться с буквы, за которой следуют буквы, цифры или символы подчеркивания.

name
: (`string`) Текст, который будет отображаться при рендеринге пункта меню.

params
: (`map`) Пользовательские свойства для пункта меню.

parent
: (`string`) `identifier` родительского пункта меню. Если `identifier` не определен, используйте `name`. Требуется для дочерних пунктов во вложенном меню.

post
: (`string`) HTML, добавляемый при отображении пункта меню.

pre
: (`string`) HTML для добавления при отображении пункта меню.

title
: (`string`) Атрибут HTML `title` отображаемого пункта меню.

weight
: (`int`) Целое ненулевое число, указывающее на позицию пункта относительно корня меню или его родителя для дочернего пункта. Более легкие пункты плавают вверху, а более тяжелые опускаются вниз.

### Пример {#example-front-matter}

Этот пункт меню первой страницы демонстрирует некоторые из доступных свойств:

```yaml
---
menus:
  main:
  - params:
      class: center
    parent: Products
    pre: <i class="fa-solid fa-code"></i>
    weight: 20
title: Software
---
```

Обратитесь к записи с помощью `site.Menus.main` в ваших шаблонах. Подробности см. в разделе [Шаблоны меню].

## Определение в конфигурации сайта

Чтобы определить пункты "главного" меню:

```yaml
menus:
  main:
  - name: Home
    pageRef: /
    weight: 10
  - name: Products
    pageRef: /products
    weight: 20
  - name: Services
    pageRef: /services
    weight: 30
```

Это создает структуру меню, к которой вы можете обращаться с помощью `site.Menus.main` в ваших шаблонах. Подробности см. в разделе [Шаблоны меню].

Чтобы определить пункты для меню "нижний колонтитул" (footer):

```yaml
menus:
  footer:
  - name: Terms
    pageRef: /terms
    weight: 10
  - name: Privacy
    pageRef: /privacy
    weight: 20
```

Это создает структуру меню, к которой вы можете обращаться с помощью `site.Menus.footer` в ваших шаблонах. Подробности см. в разделе [Шаблоны меню](https://gohugo.io/templates/menu/).

> В приведенных выше примерах ключом конфигурации является `menus`. Ключ конфигурации `menu` (единственное число) является псевдонимом для `menus`.


### Свойства {#properties-site-configuration}

> [Свойства, доступные для пунктов меню, определенных на главной странице], также доступны для пунктов меню, определенных в конфигурации сайта.

[Свойства, доступные для пунктов меню, определенных на главной странице]: /content-management/menus/#properties-front-matter

Каждый пункт меню, определенный в конфигурации сайта, требует двух или более свойств:

- Укажите `name` и `pageRef` для внутренних ссылок
- Укажите `name` и `url` для внешних ссылок

pageRef
: (`string`) Логический путь к целевой странице, относительно каталога `content`. Опустите код языка и расширение файла. Требуется для *внутренних* ссылок.

Kind|pageRef
:--|:--
home|`/`
page|`/books/book-1`
section|`/books`
taxonomy|`/tags`
term|`/tags/foo`

url
: (`string`) Требуется для *внешних* ссылок.

### Пример {#example-site-configuration}

Это вложенное меню демонстрирует некоторые из доступных свойств:

```hugo.yaml
menus:
  main:
  - name: Products
    pageRef: /products
    weight: 10
  - name: Hardware
    pageRef: /products/hardware
    parent: Products
    weight: 1
  - name: Software
    pageRef: /products/software
    parent: Products
    weight: 2
  - name: Services
    pageRef: /services
    weight: 20
  - name: Hugo
    params:
      rel: external
    pre: <i class="fa fa-heart"></i>
    url: https://gohugo.io/
    weight: 30
```

```
[[menus.main]]
name = 'Products'
pageRef = '/products'
weight = 10

[[menus.main]]
name = 'Hardware'
pageRef = '/products/hardware'
parent = 'Products'
weight = 1

[[menus.main]]
name = 'Software'
pageRef = '/products/software'
parent = 'Products'
weight = 2

[[menus.main]]
name = 'Services'
pageRef = '/services'
weight = 20

[[menus.main]]
name = 'Hugo'
pre = '<i class="fa fa-heart"></i>'
url = 'https://gohugo.io/'
weight = 30
[menus.main.params]
rel = 'external'
```

Это создает структуру меню, к которой вы можете обращаться с помощью `site.Menus.main` в ваших шаблонах. Подробности см. в разделе [Шаблоны меню].

## Локализация

Hugo предоставляет два метода локализации пунктов меню. Смотрите [мультиязычность].

## Рендер

Смотри [шаблоны меню].

[локализуйте]: /content-management/multilingual/#menus
[шаблоны меню]: /templates/menu/
[мультиязычность]: /content-management/multilingual/#menus
[раздел]: /getting-started/glossary/#section
[шаблона]: /templates/menu/
