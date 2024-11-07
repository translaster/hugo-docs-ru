---
title: "hugo config"
slug: hugo_config
url: /commands/hugo_config/
date: 2024-11-07T18:11:59+05:00
---
## hugo config

Отобразить конфигурацию сайта

### Описание

Отображение конфигурации сайта, как по-умолчанию, так и пользовательских настроек.

```
hugo config [command] [flags]
```

### Параметры

```
  -b, --baseURL string           имя хоста (и путь) к корню, напр. https://spf13.com/
      --cacheDir string          путь файловой системы к директории кэша
  -c, --contentDir string        путь файловой системы к директории контента
      --format string            предпочтительный формат файла (toml, yaml or json) (по-умолчанию "toml")
  -h, --help                     справка по конфигурации
      --lang string              язык, на котором будет отображаться конфигурация. По умолчанию выбирается первый определенный язык.
      --renderSegments strings   именованные сегменты для рендеринга (настраиваются в конфигурации сегментов)
  -t, --theme strings            используемая тема (расположена в /themes/THEMENAME/)
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
* [hugo config mounts](/commands/hugo_config_mounts/)	 - Печать настроенных монтирований файлов

