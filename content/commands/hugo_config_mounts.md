---
title: "hugo config mounts"
slug: hugo_config_mounts
url: /commands/hugo_config_mounts/
---
## hugo config mounts

Печать настроенных монтирований файлов

```
hugo config mounts [flags] [args]
```

### Параметры

```
  -b, --baseURL string           имя хоста (и путь) к корню, напр. https://spf13.com/
      --cacheDir string          путь файловой системы к каталогу кэша
  -c, --contentDir string        путь файловой системы к каталогу контента
  -h, --help                     справка по mounts
      --renderSegments strings   именованные сегменты для рендеринга (настраиваются в конфигурации сегментов)
  -t, --theme strings            используемая тема (размещается в /themes/THEMENAME/)
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

* [hugo config](/commands/hugo_config/)	 - Отобразить конфигурацию сайта

