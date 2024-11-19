---
title: "hugo completion fish"
slug: hugo_completion_fish
url: /commands/hugo_completion_fish/
date: 2024-11-11T11:46:13+05:00
draft: false

---
## hugo completion fish

Генерирует скрипт автозаполнения для  fish

### Описание

Генерирует скрипт автозаполнения для оболочки fish.

Для загрузки автозаполнений в текущей сессии оболочки:

	hugo completion fish | source

Чтобы загружать автозаполнения для каждого нового сеанса, выполните один раз:

	hugo completion fish > ~/.config/fish/completions/hugo.fish

Чтобы эта настройка вступила в силу, вам нужно будет запустить новую оболочку.


```
hugo completion fish [flags]
```

### Параметры

```
  -h, --help              справка по fish
      --no-descriptions   отключение автозаполнения описаний
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

