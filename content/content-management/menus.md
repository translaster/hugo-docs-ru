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

Use these properties when defining menu entries in front matter:

identifier
: (`string`) Required when two or more menu entries have the same `name`, or when localizing the `name` using translation tables. Must start with a letter, followed by letters, digits, or underscores.

name
: (`string`) The text to display when rendering the menu entry.

params
: (`map`) User-defined properties for the menu entry.

parent
: (`string`) The `identifier` of the parent menu entry. If `identifier` is not defined, use `name`. Required for child entries in a nested menu.

post
: (`string`) The HTML to append when rendering the menu entry.

pre
: (`string`) The HTML to prepend when rendering the menu entry.

title
: (`string`) The HTML `title` attribute of the rendered menu entry.

weight
: (`int`) A non-zero integer indicating the entry's position relative the root of the menu, or to its parent for a child entry. Lighter entries float to the top, while heavier entries sink to the bottom.

### Пример {#example-front-matter}

This front matter menu entry demonstrates some of the available properties:

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

Access the entry with `site.Menus.main` in your templates. See [menu templates] for details.

## Define in site configuration

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

This creates a menu structure that you can access with `site.Menus.main` in your templates. See [menu templates] for details.

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

This creates a menu structure that you can access with `site.Menus.footer` in your templates. See [menu templates] for details.

> The configuration key in the examples above is `menus`. The `menu` (singular) configuration key is an alias for `menus`.


### Свойства {#properties-site-configuration}


> The [properties available to entries defined in front matter] are also available to entries defined in site configuration.

[properties available to entries defined in front matter]: /content-management/menus/#properties-front-matter


Each menu entry defined in site configuration requires two or more properties:

- Specify `name` and `pageRef` for internal links
- Specify `name` and `url` for external links

pageRef
: (`string`) The logical path of the target page, relative to the `content` directory. Omit language code and file extension. Required for *internal* links.

Kind|pageRef
:--|:--
home|`/`
page|`/books/book-1`
section|`/books`
taxonomy|`/tags`
term|`/tags/foo`

url
: (`string`) Required for *external* links.

### Example {#example-site-configuration}

This nested menu demonstrates some of the available properties:

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

This creates a menu structure that you can access with `site.Menus.main` in your templates. See [menu templates] for details.

## Локализация

Hugo provides two methods to localize your menu entries. See [мультиязычность].

## Render

See [menu templates].

[локализуйте]: /content-management/multilingual/#menus
[шаблоны меню]: /templates/menu/
[мультиязычность]: /content-management/multilingual/#menus
[раздел]: /getting-started/glossary/#section
[шаблона]: /templates/menu/
