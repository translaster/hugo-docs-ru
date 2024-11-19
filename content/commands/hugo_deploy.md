---
title: "hugo deploy"
slug: hugo_deploy
url: /commands/hugo_deploy/
---
## hugo deploy

Развертывание сайта в облаке провайдера

### Описание

Развертывание сайта в облаке провайдера

Подробную документацию смотри https://gohugo.io/hosting-and-deployment/hugo-deploy/.

```
hugo deploy [flags] [args]
```

### Параметры

```
      --confirm          запрашивать подтверждение перед внесением изменений в цель
      --dryRun           холостой прогон
      --force            принудительная загрузка всех файлов
  -h, --help             справка по deploy
      --invalidateCDN    аннулировать кэш CDN, указанный в цели развертывания (по умолчанию true)
      --maxDeletes int   максимальное количество файлов для удаления, или -1 для отключения (по умолчанию 256)
      --target string    целевое развертывание из раздела deployments в файле конфигурации; по умолчанию выбирается первое
      --workers int      количество обработчиков для передачи файлов. по умолчанию 10 (по умолчанию 10)
```

### Опции, наследуемые от родительских команд

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

* [hugo](/commands/hugo/)	 - Создай свой сайт

