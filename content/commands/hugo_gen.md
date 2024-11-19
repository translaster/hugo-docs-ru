---
title: "hugo gen"
slug: hugo_gen
url: /commands/hugo_gen/
---
## hugo gen

Создание документации и стилей подсветки синтаксиса

### Описание

Создайте документацию для вашего проекта с помощью механизма документации Hugo, включая подсветку синтаксиса для различных языков программирования.

### Параметры

```
  -h, --help   help for gen
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

* [hugo](/commands/hugo/)	 - Создай свой сайт
* [hugo gen chromastyles](/commands/hugo_gen_chromastyles/)	 - Создать таблицу стилей CSS для подсветки кода Chroma
* [hugo gen doc](/commands/hugo_gen_doc/)	 - Создание документации в формате Markdown для Hugo CLI
* [hugo gen man](/commands/hugo_gen_man/)	 - Создание man-страниц для Hugo CLI

