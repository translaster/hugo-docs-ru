---
title: "hugo gen doc"
slug: hugo_gen_doc
url: /commands/hugo_gen_doc/
date: 2024-11-19T17:17:42+05:00
---
## hugo gen doc

Создание документации в формате Markdown для Hugo CLI.

### Описание

Создание документации в формате Markdown для Hugo CLI.
			Эта команда, в основном, используется для создания актуальной документации по интерфейсу командной строки Hugo для https://gohugo.io/.

	Она создает один файл в формате Markdown для каждой команды, с содержанием, подходящим для визуализации в Hugo.
```
hugo gen doc [flags] [args]
```

### Параметры

```
      --dir string   каталог для записи документации (по-умолчанию "/tmp/hugodoc/")
  -h, --help         справка для doc
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

* [hugo gen](/commands/hugo_gen/)	 - Создание документации и стилей подсветки синтаксиса

