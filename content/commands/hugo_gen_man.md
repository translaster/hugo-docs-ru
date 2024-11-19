---
title: "hugo gen man"
slug: hugo_gen_man
url: /commands/hugo_gen_man/
date: 2024-11-19T17:24:12+05:00
---
## hugo gen man

Создание man-страниц для Hugo CLI

### Описание

Эта команда автоматически генерирует актуальные man-страницы интерфейса командной строки Hugo интерфейса командной строки. По умолчанию она создает файлы man-страниц
	в каталоге «man» в текущем каталоге.

```
hugo gen man [flags] [args]
```

### Параметры

```
      --dir string   каталог для записи man-страниц (по-умолчанию "man/")
  -h, --help         справка по man
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

* [hugo gen](/commands/hugo_gen/)	 - Создание документации и стилей подсветки синтаксиса

