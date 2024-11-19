---
title: "hugo gen chromastyles"
slug: hugo_gen_chromastyles
url: /commands/hugo_gen_chromastyles/
date: 2024-11-19T17:13:37+05:00
---
## hugo gen chromastyles

Создание таблицы стилей CSS для подсветки кода Chroma

### Описание

Создание таблицы стилей CSS для подсветки кода Chroma для заданного стиля. Эта таблица стилей необходима, если в конфигурации отключен markup.highlight.noClasses.

Смотрите https://xyproto.github.io/splash/docs/all.html для предварительного просмотра доступных стилей.

```
hugo gen chromastyles [flags] [args]
```

### Параметры

```
  -h, --help                            справка по chromastyles
      --highlightStyle string           цвета переднего и заднего плана для выделенных линий, например --highlightStyle "#fff000 bg:#000fff"
      --lineNumbersInlineStyle string   цвета переднего плана и фона для номеров строк, например. --lineNumbersInlineStyle "#fff000 bg:#000fff"
      --lineNumbersTableStyle string    цвета переднего плана и фона для номеров строк таблицы, например. --lineNumbersTableStyle "#fff000 bg:#000fff"
      --style string                    стиль подсветки (смотри https://xyproto.github.io/splash/docs/) (по-умолчанию "friendly")
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

* [hugo gen](/commands/hugo_gen/)	 - Создание документации и стиль подсветки синтаксиса

