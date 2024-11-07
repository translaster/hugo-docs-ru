---
title: "hugo"
slug: hugo
url: /commands/hugo/
date: 2024-11-06T17:02:23+05:00
---
## hugo

Создайте свой сайт

### Описание

hugo - это основная команда, используемая для создания вашего сайта Hugo.

Hugo - это быстрый и гибкий генератор статических сайтов, созданный с любовью spf13 и его друзьями на языке Go.

Полная документация доступна по адресу https://gohugo.io/.

```
hugo [flags]
```

### Параметры

```
  -b, --baseURL string             имя хоста (и путь) к корню, например, https://spf13.com/.
  -D, --buildDrafts                включая содержимое, помеченное как черновик
  -E, --buildExpired               включить просроченное содержимое
  -F, --buildFuture                включать содержимое с датой публикации в будущем
      --cacheDir string            путь файловой системы к каталогу кэша
      --cleanDestinationDir        remove files from destination not found in static directories
      --clock string               set the clock used by Hugo, e.g. --clock 2021-11-06T22:30:00.00+09:00
      --config string              config file (default is hugo.yaml|json|toml)
      --configDir string           config dir (default "config")
  -c, --contentDir string          filesystem path to content directory
      --debug                      debug output
  -d, --destination string         filesystem path to write files to
      --disableKinds strings       disable different kind of pages (home, RSS etc.)
      --enableGitInfo              add Git revision, date, author, and CODEOWNERS info to the pages
  -e, --environment string         build environment
      --forceSyncStatic            copy all files when static is changed.
      --gc                         enable to run some cleanup tasks (remove unused cache files) after the build
  -h, --help                       справка по hugo
      --ignoreCache                ignores the cache directory
      --ignoreVendorPaths string   ignores any _vendor for module paths matching the given Glob pattern
  -l, --layoutDir string           filesystem path to layout directory
      --logLevel string            уровень лога (debug|info|warn|error)
      --minify                     minify any supported output format (HTML, XML etc.)
      --noBuildLock                не создавать файл .hugo_build.lock
      --noChmod                    don't sync permission mode of files
      --noTimes                    don't sync modification time of files
      --panicOnWarning             panic on first WARNING log
      --poll string                set this to a poll interval, e.g --poll 700ms, to use a poll based approach to watch for file system changes
      --printI18nWarnings          вывести отсутствующиее переводы
      --printMemoryUsage           print memory usage to screen at intervals
      --printPathWarnings          print warnings on duplicate target paths etc.
      --printUnusedTemplates       print warnings on unused templates.
      --quiet                      build in quiet mode
      --renderSegments strings     named segments to render (configured in the segments config)
  -M, --renderToMemory             render to memory (mostly useful when running the server)
  -s, --source string              filesystem path to read files relative from
      --templateMetrics            display metrics about template executions
      --templateMetricsHints       calculate some improvement hints when combined with --templateMetrics
  -t, --theme strings              themes to use (located in /themes/THEMENAME/)
      --themesDir string           filesystem path to themes directory
      --trace file                 write trace to file (not useful in general)
  -v, --verbose                    verbose output
  -w, --watch                      watch filesystem for changes and recreate as needed
```

### СМОТРИТЕ ТАКЖЕ

* [hugo build](/commands/hugo_build/)	 - Создай свой сайт
* [hugo completion](/commands/hugo_completion/)	 - Создайте скрипт автозаполнения для указанной оболочки
* [hugo config](/commands/hugo_config/)	 - Просмотр конфигурации сайта
* [hugo convert](/commands/hugo_convert/)	 - Перевести титульный лист в другой формат
* [hugo deploy](/commands/hugo_deploy/)	 - Развертывание сайта в облаке провайдера
* [hugo env](/commands/hugo_env/)	 - Отображение информации о версии и окружении
* [hugo gen](/commands/hugo_gen/)	 - Создание документации и стилей подсветки синтаксиса
* [hugo import](/commands/hugo_import/)	 - Импорт сайта из другой системы
* [hugo list](/commands/hugo_list/)	 - Список контента
* [hugo mod](/commands/hugo_mod/)	 - Управление модулями
* [hugo new](/commands/hugo_new/)	 - Создание нового содержимого
* [hugo server](/commands/hugo_server/)	 - Запуск встроенного веб-сервера
* [hugo version](/commands/hugo_version/)	 - Отобразить версию


