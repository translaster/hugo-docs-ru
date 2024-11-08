---
title: "hugo server"
slug: hugo_server
url: /commands/hugo_server/
date: 2024-11-08T10:42:36+05:00
draft: false

---
## hugo server

Запуск встроенного веб-сервера

### Описание

Hugo предоставляет свой собственный веб-сервер, который создает и обслуживает сайт.
Хотя hugo server отличается высокой производительностью, это веб-сервер с ограниченными возможностями.

Команда `hugo server` по умолчанию записывает и обслуживает файлы с диска, но вы можете выводить файлы в память, используя флаг `--renderToMemory`. Это может быть быстрее в некоторых случаях, но при этом будет потребляться больше памяти.

По умолчанию hugo также будет следить за любыми изменениями в ваших файлах и автоматически перестраивать сайт. Затем он в реальном времени перезагрузит все открытые страницы браузера и передаст туда последнее содержимое. Поскольку большинство сайтов Hugo создаются за доли секунды, вы сможете сохранить и увидеть свои изменения практически мгновенно.

```
hugo server [command] [flags]
```

### Параметры

```
      --appendPort               добавлять порт к базовому URL (по умолчанию true)
  -b, --baseURL string           имя хоста (и путь) к корню, напр. https://spf13.com/
      --bind string              интерфейс, к которому будет привязан сервер (по-умолчанию "127.0.0.1")
  -D, --buildDrafts              включая контент, помеченный как черновик (draft)
  -E, --buildExpired             включая истекший контент
  -F, --buildFuture              включая контент с датой публикации в будущем
      --cacheDir string          путь файловой системы к каталогу кэша
      --cleanDestinationDir      удалять файлы из пункта назначения, не найденные в статических каталогах
  -c, --contentDir string        путь файловой системы к каталогу контента
      --disableBrowserError      не отображать ошибки сборки в браузере
      --disableFastRender        выполнять полный рендеринг при изменениях
      --disableKinds strings     отключение различных типов страниц (главная, RSS и т.д.)
      --disableLiveReload        смотреть без включения живой перезагрузки браузера при пересборке
      --enableGitInfo            добавить информацию о ревизии Git, дате, авторе и CODEOWNERS на страницы
      --forceSyncStatic          копировать все файлы при изменении статики
      --gc                       включить выполнение некоторых задач по очистке (удаление неиспользуемых файлов кэша) после сборки
  -h, --help                     справка по server
      --ignoreCache              игнорировать каталог кэша
  -l, --layoutDir string         путь файловой системы к каталогу шаблонов
      --liveReloadPort int       порт для живой перезагрузки (т.е. 443 в ситуациях с HTTPS-прокси) (по умолчанию -1)
      --minify                   минифицировать любой поддерживаемый формат вывода (HTML, XML и т.д.)
  -N, --navigateToChanged        переход к измененному файлу содержимого при перезагрузке браузера
      --noBuildLock              не создавать файл .hugo_build.lock
      --noChmod                  не синхронизируйте режим разрешения файлов
      --noHTTPCache              предотвращение кэширования HTTP
      --noTimes                  не синхронизировать время модификации файлов
      --panicOnWarning           паника при первом журнале WARNING
      --poll string              установить значение интервала опроса, например --poll 700ms, чтобы использовать подход, основанный на опросе, для отслеживания изменений в файловой системе
  -p, --port int                 порт, который будет слушивать сервер (по умолчанию 1313)
      --pprof                    включить сервер pprof (порт 8080)
      --printI18nWarnings        печать отсутствующих переводов
      --printMemoryUsage         выводить данные об использовании памяти на экран через определенные интервалы
      --printPathWarnings        выводить предупреждения о дублировании целевых путей и т.д.
      --printUnusedTemplates     выводить предупреждения о неиспользуемых шаблонах.
      --renderSegments strings   именованные сегменты для рендеринга (настраиваются в конфигурации сегментов)
      --renderStaticToDisk       обслуживать статические файлы с диска и динамические файлы из памяти
      --templateMetrics          отображение метрик о выполнении шаблонов
      --templateMetricsHints     вычислить некоторые подсказки по улучшению в сочетании с --templateMetrics
  -t, --theme strings            используемая тема (расположена в /themes/THEMENAME/)
      --tlsAuto                  генерировать и использовать локально доверенные сертификаты
      --tlsCertFile string       путь к файлу сертификата TLS
      --tlsKeyFile string        путь к файлу ключа TLS
      --trace file               записывать трассировку в файл (в общем случае бесполезно)
  -w, --watch                    следить за изменениями в файловой системе и пересоздавать ее по мере необходимости (по умолчанию true)
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

* [hugo](/commands/hugo/)	 - Собери свой сайт
* [hugo server trust](/commands/hugo_server_trust/)	 - Установка локального CA в доверенное хранилище системы.


