---
title: "hugo server trust"
slug: hugo_server_trust
url: /commands/hugo_server_trust/
date: 2024-11-08T10:42:45+05:00
draft: false

---
## hugo server trust

Устанавливает локальный CA в доверенное хранилище системы.

```
hugo server trust [flags] [args]
```

### Параметры

```
  -h, --help        справка по trust
      --uninstall   Убрать локальный CA (но не удалять его).
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

* [hugo server](/commands/hugo_server/)	 - Запуск встроенного веб-сервера

