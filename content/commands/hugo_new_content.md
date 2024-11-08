---
title: "hugo new content"
slug: hugo_new_content
url: /commands/hugo_new_content/
date: 2024-11-08T09:44:21+05:00
---
## hugo new content

Создает новый контент

### Описание

Создает новый файл с содержимым и автоматически устанавливает дату и заголовок.
Она сама определит, какой тип файла создать, исходя из указанного пути.

Вы также можете указать тип с помощью `-k KIND`.

Если в вашей теме или сайте есть архетипы, они будут использованы.

Убедитесь, что вы запустили эту программу в корневом каталоге вашего сайта.

```
hugo new content [path] [flags]
```

### Параметры

```
  -b, --baseURL string           hostname (and path) to the root, e.g. https://spf13.com/
      --cacheDir string          filesystem path to cache directory
  -c, --contentDir string        filesystem path to content directory
      --editor string            редактировать новый контент с помощью этого редактора, если присутствует в системе
  -f, --force                    заменить файл если он уже существует
  -h, --help                     help for content
  -k, --kind string              тип контента при создании
      --renderSegments strings   named segments to render (configured in the segments config)
  -t, --theme strings            используемая тема (располагается в /themes/THEMENAME/)
```

### Параметры, наследуемые от родительских команд

```
      --clock string               set the clock used by Hugo, e.g. --clock 2021-11-06T22:30:00.00+09:00
      --config string              config file (default is hugo.yaml|json|toml)
      --configDir string           config dir (default "config")
      --debug                      debug output
  -d, --destination string         filesystem path to write files to
  -e, --environment string         build environment
      --ignoreVendorPaths string   ignores any _vendor for module paths matching the given Glob pattern
      --logLevel string            log level (debug|info|warn|error)
      --quiet                      build in quiet mode
  -M, --renderToMemory             render to memory (mostly useful when running the server)
  -s, --source string              filesystem path to read files relative from
      --themesDir string           filesystem path to themes directory
  -v, --verbose                    verbose output
```

### СМОТРИ ТАКЖЕ

* [hugo new](/commands/hugo_new/)	 - Создать новый контент

