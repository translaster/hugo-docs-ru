---
title: "hugo import jekyll"
slug: hugo_import_jekyll
url: /commands/hugo_import_jekyll/
---
## hugo import jekyll

hugo import для Jekyll

### Описание

hugo import для Jekyll.
		
Импорт из Jekyll требует двух путей, например, `hugo import jekyll jekyll_root_path target_path`.

```
hugo import jekyll [flags] [args]
```

### Параметры

```
      --force   разрешить импорт в непустой целевой каталог
  -h, --help    справка по jekyll
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

* [hugo import](/commands/hugo_import/)	 - Импорт сайта из другой системы

