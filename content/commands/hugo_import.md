---
title: "hugo import"
slug: hugo_import
url: /commands/hugo_import/
---
## hugo import

Импорт сайта из другой системы

### Synopsis

Импорт сайта из другой системы.

Импорт требует подкоманды, например, `hugo import jekyll jekyll_root_path target_path`.

### Параметры

```
  -h, --help   справка по import
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

### СМОТРИТЕ ТАКЖЕ

* [hugo](/commands/hugo/)	 - Создай свой сайт
* [hugo import jekyll](/commands/hugo_import_jekyll/)	 - hugo import from Jekyll

