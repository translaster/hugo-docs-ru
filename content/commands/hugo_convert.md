---
title: "hugo convert"
slug: hugo_convert
url: /commands/hugo_convert/
---
## hugo convert

Конвертировать титульную страницу в другой формат

### Описание

Преобразование титульной страницы в другой формат.

Дополнительные сведения см. в подкомандах convert toJSON, toTOML и toYAML.

### Параметры

```
  -h, --help            справка по convert
  -o, --output string   путь для записи файлов
      --unsafe          для снижения безопасности операций сначала создайте резервную копию
```

### Опции, наследуемые от родительских команд

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
* [hugo convert toJSON](/commands/hugo_convert_tojson/)	 - Конвертировать титульную страницу в JSON
* [hugo convert toTOML](/commands/hugo_convert_totoml/)	 - Конвертировать титульную страницу в TOML
* [hugo convert toYAML](/commands/hugo_convert_toyaml/)	 - Конвертировать титульную страницу в YAML

