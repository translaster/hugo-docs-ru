---
title: "hugo new"
slug: hugo_new
url: /commands/hugo_new/
date: 2024-11-08T09:39:27+05:00
---
## hugo new

Создает новый контент

### Описание

Создайте новый файл с содержимым и автоматически установите дату и заголовок.
Он сам определит, какой тип файла создать, исходя из указанного пути.

Вы также можете указать тип с помощью `-k KIND`.

Если в вашей теме или сайте есть архетипы, они будут использованы.

Убедитесь, что вы запустили эту программу в корневом каталоге вашего сайта.

### Параметры

```
  -h, --help   справка по new
```

### Параметры, наследуемые от родительских команд

```
      --clock string               set the clock used by Hugo, e.g. --clock 2021-11-06T22:30:00.00+09:00
      --config string              файл конфигурации (по-умолчанию hugo.yaml|json|toml)
      --configDir string           каталог конфигурации (по-умолчанию "config")
      --debug                      debug output
  -d, --destination string         путь файловой системы для записи файлов
  -e, --environment string         среда сборки
      --ignoreVendorPaths string   ignores any _vendor for module paths matching the given Glob pattern
      --logLevel string            уровень журнала (debug|info|warn|error)
      --quiet                      сборка в тихом режиме
  -M, --renderToMemory             render to memory (mostly useful when running the server)
  -s, --source string              filesystem path to read files relative from
      --themesDir string           filesystem path to themes directory
  -v, --verbose                    verbose output
```

### СМОТРИ ТАКЖЕ

* [hugo](/commands/hugo/)	 - Создай свой сайт
* [hugo new content](/commands/hugo_new_content/)	 - Создать новый контент
* [hugo new site](/commands/hugo_new_site/)	 - Создать новый сайт (каркас)
* [hugo new theme](/commands/hugo_new_theme/)	 - Создать новую тему (каркас)

