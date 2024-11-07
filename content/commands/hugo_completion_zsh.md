---
title: "hugo completion zsh"
slug: hugo_completion_zsh
url: /commands/hugo_completion_zsh/
date: 2024-11-07T18:05:32+05:00
---
## hugo completion zsh

Создаём скрипт автозаполнения для zsh

### Описание

Создайте скрипт автозаполнения для оболочки zsh

Если запуск для вашей оболочки еще не включено в вашей среде, то нужно включить его. Вы можете один раз выполнить следующее:

	echo "autoload -U compinit; compinit" >> ~/.zshrc

Чтобы выполнить запуск в текущем сеансе оболочки:

	source <(hugo completion zsh)

Чтобы загрузить запуск для каждой новой сессии, выполните один раз:

#### Linux:

	hugo completion zsh > "${fpath[1]}/_hugo"

#### macOS:

	hugo completion zsh > $(brew --prefix)/share/zsh/site-functions/_hugo

Чтобы эта настройка вступила в силу, вам нужно будет запустить новую оболочку.


```
hugo completion zsh [flags]
```

### Параметры

```
  -h, --help              справка для zsh
      --no-descriptions   отключение описаний выполнения
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

* [hugo completion](/commands/hugo_completion/)	 - Создайте скрипт автозаполнения для указанной оболочки

