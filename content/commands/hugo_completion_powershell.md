---
title: "hugo completion powershell"
slug: hugo_completion_powershell
url: /commands/hugo_completion_powershell/
date: 2024-11-11T11:49:32+05:00
---
## hugo completion powershell

Создает скрипт автозаполнения для powershell

### Описание

Создает скрипт автозаполнения для powershell.

Для загрузки автозаполнений в текущем сеансе оболочки:

	hugo completion powershell | Out-String | Invoke-Expression.

Чтобы загружать автозаполнения для каждого нового сеанса, добавьте вывод приведенной выше команды в свой профиль powershell.

```
hugo completion powershell [flags]
```

### Параметры

```
  -h, --help              справка по powershell
      --no-descriptions   отключить автозаполнения описаний
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

* [hugo completion](/commands/hugo_completion/)	 - Создать скрипт автозаполнения для указанной оболочки

