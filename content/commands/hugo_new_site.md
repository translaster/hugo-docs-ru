---
title: "hugo new site"
slug: hugo_new_site
url: /commands/hugo_new_site/
date: 2024-11-08T10:17:45+05:00
---
## hugo new site

Создать новый сайт (каркас)

### Описание

Создаёт новый сайт в указанном каталоге.
Новый сайт будет иметь правильную структуру, но без контента и темы.
Используйте `hugo new [contentPath]` для создания нового контента.

```
hugo new site [path] [flags]
```

### Параметры

```
  -f, --force           инициализация внутри непустого каталога
      --format string   предпочтительный формат файлов (toml, yaml или json) (по-умолчанию "toml")
  -h, --help            справка по site
```

### Опции, наследуемые от родительских команд

```
      --clock string               set the clock used by Hugo, e.g. --clock 2021-11-06T22:30:00.00+09:00
      --config string              файл конфигурации (по-умолчанию hugo.yaml|json|toml)
      --configDir string           каталог конфигурации (по-умолчанию "config")
      --debug                      debug output
  -d, --destination string         filesystem path to write files to
  -e, --environment string         среда сборки
      --ignoreVendorPaths string   ignores any _vendor for module paths matching the given Glob pattern
      --logLevel string            уровень лога (debug|info|warn|error)
      --quiet                      сборка в тихом режиме
  -M, --renderToMemory             render to memory (mostly useful when running the server)
  -s, --source string              filesystem path to read files relative from
      --themesDir string           filesystem path to themes directory
  -v, --verbose                    детальность вывода
```

### СМОТРИ ТАКЖЕ

* [hugo new](/commands/hugo_new/)	 - Создать новый контент

