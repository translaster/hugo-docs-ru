---
title: "hugo version"
slug: hugo_version
url: /commands/hugo_version/
date: 2024-11-08T10:40:30+05:00
draft: false

---
## hugo version

Отображает версию

### Описание

Отображение информации о версии и окружении. Это полезно для сообщений об ошибках в Hugo.

```
hugo version [flags] [args]
```

### Параметры

```
  -h, --help   справка по version
```

### Параметры, наследуемые от родительских команд

```
      --clock string               установка часов используя Hugo, напр. --clock 2021-11-06T22:30:00.00+09:00
      --config string              файл конфигурации (по-умолчанию hugo.yaml|json|toml)
      --configDir string           каталог конфигурации (по-умолчанию "config")
      --debug                      вывод отладки
  -d, --destination string         путь файловой системы для записи файлов в
  -e, --environment string         среда сборки
      --ignoreVendorPaths string   игнорировать любые _vendor для путей модулей, соответствующих заданному шаблону Glob
      --logLevel string            уровень лога (debug|info|warn|error)
      --quiet                      сборка в тихом режиме
  -M, --renderToMemory             рендеринг в память (в основном полезно при запуске сервера)
  -s, --source string              путь для чтения файлов относительно
      --themesDir string           путь к каталогу тем
  -v, --verbose                    детальность вывода
```

### СМОТРИ ТАКЖЕ

* [hugo](/commands/hugo/)	 - Создай свой сайт

