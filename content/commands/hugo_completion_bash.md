---
title: "hugo completion bash"
slug: hugo_completion_bash
url: /commands/hugo_completion_bash/
date: 2024-11-11T11:40:58+05:00
draft: false
---
## hugo completion bash

Генерирует скрипт автозаполнения для bash

### Описание

Генерирует скрипт автозаполнения для оболочки bash.

Этот скрипт зависит от пакета 'bash-completion'.
Если он еще не установлен, вы можете установить его через менеджер пакетов вашей ОС.

Чтобы загрузить автозаполнение в текущей сессии оболочки:

	source <(hugo completion bash)

Чтобы загрузить завершения для каждого нового сеанса, выполните один раз:

#### Linux:

	hugo completion bash > /etc/bash_completion.d/hugo

#### macOS:

	hugo completion bash > $(brew --prefix)/etc/bash_completion.d/hugo

Чтобы эта настройка вступила в силу, вам нужно будет запустить новую оболочку.


```
hugo completion bash
```

### Параметры

```
  -h, --help              справка для bash
      --no-descriptions   отключение функции завершения
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

