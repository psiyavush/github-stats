# Статистика GitHub для Readme файлов

Получите динамически сгенерированную статистику GitHub в своих файлах README!

Вы можете их использовать:
- Во всех README своих проектов, для отображение статистических данных проекта.
Такая карточка, покажет интересную и информативную статистику вашего проекта. Подчеркнет его особенности и покажет в целом проделанную вами работу.

![github-stats repo info](https://github-readme-stats.vercel.app/api/pin/?username=anuraghazra&repo=github-readme-stats)
Посмотреть [все версии](#все-демо)
- Для оформления своего профиля на GitHub
Красивые карточки (баннеры, информеры) статистики вашего профиля на GitHub. Вывод такой статистики украсит оформление вашего профиля на GitHub. А благодаря огромному количеству различных тем и настроек, позволит сделать ваш профиль на GitHub индивидуальным, ярким и запоминающемся.

|![Anurag's GitHub stats](https://github-stats-psiyavushs-projects.vercel.app/api?username=anuraghazra\&show_icons=true\&theme=radical&locale=ru&cache_seconds=86400) |![Top Langs](https://github-stats-psiyavushs-projects.vercel.app/api/top-langs/?username=anuraghazra&layout=compact&langs_count=8&card_width=400&locale=ru&cache_seconds=86400)|
| ------------- | -------------

Посмотреть [все версии](#все-демо)

Это русскоязычная адаптация проекта [github-readme-stats](https://github.com/anuraghazra/github-readme-stats/)

## Оглавление
- [Карточка статистики GitHub](#карточка-статистики-github)
    - [Скрытие индивидуальной статистики](#скрытие-индивидуальной-статистики)
    - [Показ дополнительной индивидуальной статистики](#показ-дополнительной-индивидуальной-статистики)
    - [Показ значков](#показ-значков)
    - [Темы](#Темы)
    - [Настройка](#настройка)
- [Дополнительные пины GitHub](#дополнительные-пины-github)
- [GitHub Extra Пины](#github-gist-пины)
- [Карточка Топ языков](#карточка-топ-языков)
- [Карточка статистики WakaTime](#карточка-статистики-wakatime)
- [Все версии карточек](#все-демо)
- [Самостоятельное развертывание проекта](#самостоятельное-развертывание-проекта)
  - [Отключить защиту ограничения скорости](#отключить-защиту-ограничения-скорости)
  - [Поддерживайте актуальность своего fork](#поддерживайте-актуальность-своего-fork)

## Важные уведомления <!-- omit in toc -->

> [!ВАЖНО]\
> Поскольку API GitHub [допускает только 5 тыс. запросов в час на учетную запись пользователя](https://docs.github.com/en/graphql/overview/resource-limitations), публичный экземпляр Vercel, размещенный на `https://github-stats-psiyavushs-projects.vercel.app/api` может столкнуться с ограничением скорости. Мы используем кэширование, чтобы этого не произошло. Вы можете отключить эти средства защиты от ограничения скорости, развернув [собственный экземпляр Vercel](#отключить-защиту-ограничения-скорости).

## Карточка статистики GitHub

Все очень просто! Скопируйте и вставьте это в свой markdown, и все.

Измените значение `?username=` на свое имя пользователя GitHub.

```md
[![Anurag's GitHub stats](https://github-stats-psiyavushs-projects.vercel.app/api?username=anuraghazra)](https://github.com/psiyavush/github-stats)
```

> [!ПРЕДУПРЕЖДЕНИЕ]\
> По умолчанию карта статистики показывает только статистику, такую ​​как звезды, коммиты и запросы на извлечение из публичных репозиториев. Чтобы отобразить приватную статистику на карте статистики, вам следует [развернуть собственный экземпляр,](#самостоятельное-развертывание-проекта) используя собственный токен API GitHub.

> [!Примечание]\
> Доступные ранги: S (top 1%), A+ (12.5%), A (25%), A- (37.5%), B+ (50%), B (62.5%), B- (75%), C+ (87.5%) and C (everyone). Эта схема ранжирования основана на [японской академической системе оценок](https://wikipedia.org/wiki/Academic_grading_in_Japan). Глобальный процент рассчитывается как взвешенная сумма процентов для каждой статистики (количество коммитов, запросов на извлечение, обзоров, проблем, звезд и подписчиков) на основе кумулятивной функции распределения  [экспоненциального](https://wikipedia.org/wiki/exponential_distribution) и [логнормального ](https://wikipedia.org/wiki/Log-normal_distribution) распределений. Реализацию можно изучить на [src/calculateRank.js](https://github.com/psiyavush/github-stats/blob/main/src/calculateRank.js). 

### Скрытие индивидуальной статистики

Вы можете передать параметр запроса `&hide=` чтобы скрыть определенную статистику со значениями, разделенными запятыми.

> Options: `&hide=stars,commits,prs,issues,contribs`

```md
![Anurag's GitHub stats](https://github-stats-psiyavushs-projects.vercel.app/api?username=anuraghazra&hide=contribs,prs)
```

### Показ дополнительной индивидуальной статистики

Вы можете передать параметр запроса `&show=` чтобы отобразить любую конкретную дополнительную статистику со значениями, разделенными запятыми.

> Options: `&show=reviews,discussions_started,discussions_answered,prs_merged,prs_merged_percentage`

```md
![Anurag's GitHub stats](https://github-stats-psiyavushs-projects.vercel.app/api?username=anuraghazra&show=reviews,discussions_started,discussions_answered,prs_merged,prs_merged_percentage)
```

### Показ значков

Чтобы включить значки, вы можете передать `&show_icons=true` параметр запроса, например так:

```md
![Anurag's GitHub stats](https://github-stats-psiyavushs-projects.vercel.app/api?username=anuraghazra&show_icons=true)
```

### Темы

Благодаря встроенным темам вы можете настроить внешний вид карточки без выполнения какой-либо [ручной настройки](#настройка).

Используйте `&theme=THEME_NAME` следующим образом:

```md
![Anurag's GitHub stats](https://github-stats-psiyavushs-projects.vercel.app/api?username=anuraghazra&show_icons=true&theme=radical)
```

#### Все встроенные темы

Github Stats поставляется с несколькими встроенными темами (например `dark`, `radical`, `merko`, `gruvbox`, `tokyonight`, `onedark`, `cobalt`, `synthwave`, `highcontrast`, `dracula`).

<img src="https://camo.githubusercontent.com/166adcf892a44c18c2ec02b4a1407de460cd2d3acc2e3e758551d75960fc04cc/68747470733a2f2f7265732e636c6f7564696e6172792e636f6d2f616e7572616768617a72612f696d6167652f75706c6f61642f76313539353137343533362f6772732d7468656d65735f6c34796e6a612e706e67" alt="Github Stats Темы" width="600px"/>

Вы можете предварительно просмотреть [все доступные Темы](themes/README.md) или проверить [файл конфигурации темы](themes/index.js). Обратите внимание, что мы приостановили добавление новых тем, чтобы уменьшить усилия по обслуживанию; все запросы на извлечение, связанные с новыми темами, будут закрыты.

#### Тема адаптивной карточки

[![Anurag's GitHub stats-Dark](https://github-stats-psiyavushs-projects.vercel.app/api?username=anuraghazra\&show_icons=true\&theme=dark#gh-dark-mode-only)](https://github.com/psiyavush/github-stats#responsive-card-theme#gh-dark-mode-only)
[![Anurag's GitHub stats-Light](https://github-stats-psiyavushs-projects.vercel.app/api?username=anuraghazra\&show_icons=true\&theme=default#gh-light-mode-only)](https://github.com/psiyavush/github-stats#responsive-card-theme#gh-light-mode-only)

Поскольку GitHub повторно загрузит карточки и будет обслуживать их из своего [CDN](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/about-anonymized-urls), мы не можем вывести тему браузера/GitHub на стороне сервера. Однако есть четыре метода, которые вы можете использовать для создания динамических тем на стороне клиента.

##### Используйте прозрачную тему

Мы включили `transparent` тему с прозрачным фоном. Эта тема оптимизирована для хорошего вида на темных и светлых темах GitHub по умолчанию. Вы можете включить эту тему с помощью параметра `&theme=transparent` например:

```md
![Anurag's GitHub stats](https://github-stats-psiyavushs-projects.vercel.app/api?username=anuraghazra&show_icons=true&theme=transparent)
```

##### Добавить прозрачный альфа-канал в тему bg\_color

Вы можете использовать `bg_color` чтобы сделать любую из [доступных тем](themes/README.md) прозрачной. Это делается путем установки `bg_color` цвета с прозрачным альфа-каналом (т.е. `bg_color=00000000`):

```md
![Anurag's GitHub stats](https://github-stats-psiyavushs-projects.vercel.app/api?username=anuraghazra&show_icons=true&bg_color=00000000)
```

##### Используйте контекстный тег темы GitHub

Вы можете использовать теги [контекста темы GitHub ](https://github.blog/changelog/2021-11-24-specify-theme-context-for-images-in-markdown/) для автоматического переключения темы на основе пользовательской темы GitHub. Это делается путем добавления `#gh-dark-mode-only` или `#gh-light-mode-only` в конец URL-адреса изображения. Этот тег будет определять, будет ли изображение, указанное в разметке, показываться только зрителям, использующим светлую или темную тему GitHub:

```md
[![Anurag's GitHub stats-Dark](https://github-stats-psiyavushs-projects.vercel.app/api?username=anuraghazra&show_icons=true&theme=dark#gh-dark-mode-only)](https://github.com/psiyavush/github-stats#gh-dark-mode-only)
[![Anurag's GitHub stats-Light](https://github-stats-psiyavushs-projects.vercel.app/api?username=anuraghazra&show_icons=true&theme=default#gh-light-mode-only)](https://github.com/psiyavush/github-stats#gh-light-mode-only)
```

##### Используйте новую медиа-функцию GitHub

Вы можете использовать [новую функцию GitHub media](https://github.blog/changelog/2022-05-19-specify-theme-context-for-images-in-markdown-beta/) в HTML, чтобы указать, отображать ли изображения для светлых или темных тем. Это делается с помощью элемента HTML `<picture>` в сочетании с функцией media `prefers-color-scheme`

```html
<picture>
  <source
    srcset="https://github-stats-psiyavushs-projects.vercel.app/api?username=anuraghazra&show_icons=true&theme=dark"
    media="(prefers-color-scheme: dark)"
  />
  <source
    srcset="https://github-stats-psiyavushs-projects.vercel.app/api?username=anuraghazra&show_icons=true"
    media="(prefers-color-scheme: light), (prefers-color-scheme: no-preference)"
  />
  <img src="https://github-stats-psiyavushs-projects.vercel.app/api?username=anuraghazra&show_icons=true" />
</picture>
```

### Настройка

Вы можете настроить внешний вид всех своих карточек по своему усмотрению с помощью параметров URL.

#### Общие параметры

| Имя | Описание | Тип | Значение по умолчанию |
| --- | --- | --- | --- |
| `title_color` | Цвет названия карточки. | string (hex color) | `2f80ed` |
| `text_color` | Цвет основного текста. | string (hex color) | `434d58` |
| `icon_color` | Цвет иконок, если доступен. | string (hex color) | `4c71f2` |
| `border_color` | Цвет границы карточки. Не применяется, если включен `hide_border` | string (hex color) | `e4e2e2` |
| `bg_color` | Цвет фона карточки. | string (hex color or a gradient in the form of *angle,start,end*) | `fffefe` |
| `hide_border` | Скрывает границу карточки. | boolean | `false` |
| `theme` | Название темы, выберите из [Все доступные Темы](themes/README.md). | enum | `default` |
| `cache_seconds` | Устанавливает заголовок кэша вручную (мин.: 21600, макс.: 86400). (min: 21600, max: 86400). | integer | `21600` |
| `locale` | Устанавливает язык в карточке, полный список доступных языков можно проверить [здесь](#доступные-языки). | enum | `en` |
| `border_radius` | Закругление углов на карточке. | number | `4.5` |

##### Градиент в bg\_color

Вы можете указать несколько значений, разделенных запятыми, в параметре bg_color для визуализации градиента в следующем формате:

    &bg_color=DEG,COLOR1,COLOR2,COLOR3...COLOR10

##### Доступные языки

Вот список всех доступных локалей:

<table>
<tr><td>

| Code | Locale |
| --- | --- |
| `cn` | Chinese |
| `zh-tw` | Chinese (Taiwan) |
| `ar` | Arabic |
| `cs` | Czech |
| `de` | German |
| `en` | English |
| `bn` | Bengali |
| `es` | Spanish |
| `fr` | French |
| `hu` | Hungarian |

</td><td>

| Code | Locale |
| --- | --- |
| `it` | Italian |
| `ja` | Japanese |
| `kr` | Korean |
| `nl` | Dutch |
| `pt-pt` | Portuguese (Portugal) |
| `pt-br` | Portuguese (Brazil) |
| `np` | Nepali |
| `el` | Greek |
| `ru` | Russian |
| `uk-ua` | Ukrainian |

</td><td>

| Code | Locale |
| --- | --- |
| `id` | Indonesian |
| `ml` | Malayalam |
| `my` | Burmese |
| `sk` | Slovak |
| `tr` | Turkish |
| `pl` | Polish |
| `uz` | Uzbek |
| `vi` | Vietnamese |
| `se` | Swedish |

</td></tr>
</table>

#### Эксклюзивные опции карты статистики

| Имя | Описание | Тип | Значение по умолчанию |
| --- | --- | --- | --- |
| `hide` | Скрывает [указанные элементы](#скрытие-индивидуальной-статистики) из статистики. | string (comma-separated values) | `null` |
| `hide_title` | Скрывает название вашей статистической карточки. | boolean | `false` |
| `card_width` | Устанавливает ширину карты вручную. | number | `500px  (approx.)` |
| `hide_rank` | Скрывает ранг и автоматически изменяет ширину карточки. | boolean | `false` |
| `rank_icon` | Показывает альтернативный значок ранга (например `github`, `percentile` или `default`). | enum | `default` |
| `show_icons` | 	Показывает значки возле всех показателей. | boolean | `false` |
| `include_all_commits` | Подсчитывайте общее количество коммитов, а не только коммиты за текущий год. | boolean | `false` |
| `line_height` | Устанавливает высоту строки между текстом. | integer | `25` |
| `exclude_repo` | Исключает указанные репозитории. | string (comma-separated values) | `null` |
| `custom_title` | Устанавливает пользовательское название для карты. | string | `<username> GitHub Stats` |
| `text_bold` | Использует жирный текст. | boolean | `true` |
| `disable_animations` | Отключает все анимации на карточке. | boolean | `false` |
| `ring_color` | Цвет круга рангов. | string (hex color) | `2f80ed` |
| `number_format` | Переключение между двумя доступными форматами отображения значений карт  `short` (например `6.6k`) и `long` (например `6626`). | enum | `short` |
| `show` | Показывает [дополнительные элементы](#показ-дополнительной-индивидуальной-статистики) на карточке статистики (например `reviews`, `discussions_started`, `discussions_answered`, `prs_merged` или`prs_merged_percentage`). | string (comma-separated values) | `null` |

> [!Примечание]\
> Если  hide\_rank=`true`, минимальная ширина карточки составляет 270 пикселей + длина заголовка и отступы.

#### Эксклюзивные возможности карточки Репозитория

| Имя | Описание | Тип | Значение по умолчанию |
| --- | --- | --- | --- |
| `show_owner` | Показывает имя владельца репозитория. | boolean | `false` |
| `description_lines_count` | Вручную задайте количество строк для описания. Указанное значение будет ограничено диапазоном от 1 до 3. Если этот параметр не указан, количество строк будет автоматически скорректировано в соответствии с фактической длиной описания. | number | `null` |

#### Эксклюзивные опции Gist Card

| Имя | Описание | Тип | Значение по умолчанию |
| --- | --- | --- | --- |
| `show_owner` | Показывает имя владельца | boolean | `false` |

#### Эксклюзивные возможности карточки языков программирования

| Имя | Описание | Тип | Значение по умолчанию |
| --- | --- | --- | --- |
| `hide` | Скрывает [указанные языки](#hide-individual-languages) from card. | string (comma-separated values) | `null` |
| `hide_title` | 	Скрывает название вашей карты. | boolean | `false` |
| `layout` | Переключение между пятью доступными раскладками `normal` & `compact` & `donut` & `donut-vertical` & `pie`. | enum | `normal` |
| `card_width` | Устанавливает ширину карты вручную. | number | `300` |
| `langs_count` | Показывает больше языков на карточке, от 1 до 20. | integer | `5` for `normal` and `donut`, `6` for other layouts |
| `exclude_repo` | Исключает указанные репозитории. | string (comma-separated values) | `null` |
| `custom_title` | Устанавливает пользовательское название для карты. | string | `Most Used Languages` |
| `disable_animations` | Отключает все анимации на карточке. | boolean | `false` |
| `hide_progress` | Использует опцию компактного макета, скрывает проценты и удаляет полосы. | boolean | `false` |
| `size_weight` | Настраивает алгоритм статистики языка (см. [Алгоритм статистики языка](#алгоритм-статистики-языка)). | integer | `1` |
| `count_weight` | Настраивает алгоритм статистики языка (см. [Алгоритм статистики языка](#алгоритм-статистики-языка)). | integer | `0` |

> [!ПРЕДУПРЕЖДЕНИЕ]\
> Названия языков должны быть экранированы URI, как указано в[Percent Encoding](https://en.wikipedia.org/wiki/Percent-encoding)
> (т. е.: `c++` должен стать `c%2B%2B`, `jupyter notebook` должен стать `jupyter%20notebook`, и т. д.). Вы можете использовать
> [urlencoder.org](https://www.urlencoder.org/) чтобы сделать это автоматически.

#### Эксклюзивные возможности карты WakaTime

| Имя | Описание | Тип | Значение по умолчанию |

| --- | --- | --- | --- |

| `hide` | Скрывает указанные в карточке языки. | string (comma-separated values) | `null` |
| `hide_title` | Скрывает название вашей карты. | boolean | `false` |
| `line_height` | Устанавливает высоту строки между текстом. | integer | `25` |
| `hide_progress` | Скрывает индикатор выполнения и процент. | boolean | `false` |
| `custom_title` | Устанавливает пользовательское название для карты. | string | `WakaTime Stats` |
| `layout` | Переключение между двумя доступными макетами `default` & `compact`. | enum | `default` |
| `langs_count` | Ограничивает количество языков на карте, по умолчанию используются все указанные языки. | integer | `null` |
| `api_domain` | Устанавливает пользовательский домен API для карты, например, для использования таких сервисов, как [Hakatime](https://github.com/mujx/hakatime) или [Wakapi](https://github.com/muety/wakapi) | string | `wakatime.com` |
| `display_format` | Устанавливает формат отображения статистики WakaTime. Выберите `time` отображение статистики на основе времени или  `percent` отображение процентов. | enum | `time` |
| `disable_animations` | Отключает все анимации на карточке. | boolean | `false` |

***

## Дополнительные пины GitHub

Дополнительные закреплённые элементы GitHub позволяют вам закрепить более 6 репозиториев в вашем профиле с помощью профиля GitHub readme.

Ура! Вы больше не ограничены 6 закрепленными репозиториями.

### Использование

Скопируйте и вставьте этот код в файл readme и измените ссылки.

Конечная точка: `api/pin?username=anuraghazra&repo=github-readme-stats`

```md
[![Readme Card](https://github-stats-psiyavushs-projects.vercel.app/api/pin/?username=anuraghazra&repo=github-readme-stats)](https://github.com/psiyavush/github-stats)
```

### Демо

![Readme Card](https://github-stats-psiyavushs-projects.vercel.app/api/pin/?username=anuraghazra\&repo=github-readme-stats&cache_seconds=86400)

Используйте параметр запроса  [show\_owner](#эксклюзивные-возможности-карты-repo) , чтобы включить имя пользователя владельца репозитория. owner username

![Readme Card](https://github-stats-psiyavushs-projects.vercel.app/api/pin/?username=anuraghazra\&repo=github-readme-stats\&show_owner=true&cache_seconds=86400)

# GitHub Gist Пины

Закрепления GitHub Gist позволяют закреплять Gist в вашем профиле GitHub с помощью профиля GitHub Readme.

### Использование

Скопируйте и вставьте этот код в файл readme и измените ссылки.

Endpoint: `api/gist?id=bbfce31e0217a3689c8d961a356cb10d`

```md
[![Gist Card](https://github-stats-psiyavushs-projects.vercel.app/api/gist?id=bbfce31e0217a3689c8d961a356cb10d)](https://gist.github.com/Yizack/bbfce31e0217a3689c8d961a356cb10d/)
```

### Демо

![Gist Card](https://github-stats-psiyavushs-projects.vercel.app/api/gist?id=bbfce31e0217a3689c8d961a356cb10d&cache_seconds=86400)

Используйте параметр запроса [show\_owner](#эксклюзивные-опции-gist-card), чтобы включить имя пользователя владельца gist.

![Gist Card](https://github-stats-psiyavushs-projects.vercel.app/api/gist?id=bbfce31e0217a3689c8d961a356cb10d\&show_owner=true&cache_seconds=86400)

# Карточка ТОП языков

Карточка основных языков показывает наиболее часто используемые языки пользователя GitHub.

> [!ПРЕДУПРЕЖДЕНИЕ]\
> По умолчанию языковая карта показывает результаты языков только из публичных репозиториев. Чтобы включить языки, используемые в частных репозиториях, вам следует [развернуть собственный экземпляр](#самостоятельное-развертывание-проекта) используя собственный токен API GitHub.

> [!Примечание]\
> Top Languages ​​не указывает уровень навыков пользователя или что-то в этом роде; это метрика GitHub для определения языков, имеющих больше всего кода на GitHub. Это новая функция github-stats.

> [!ПРЕДУПРЕЖДЕНИЕ]\
> Эта карта показывает использование языка только внутри ваших собственных нефоркнутых репозиториев, независимо от того, кто является автором коммитов. Она не включает ваши вклады в репозитории других пользователей/организаций. В настоящее время нет способа получить эти данные из API GitHub.

> [!ПРЕДУПРЕЖДЕНИЕ]\
> В настоящее время эта карта показывает данные только о первых 100 репозиториях. Это связано с ограничениями API GitHub, которые вызывают простои публичных экземпляров. В будущем это поведение будет улучшено путем освобождения действия GitHub или предоставления переменных среды для собственных экземпляров пользователя.

### Использование

Скопируйте и вставьте этот код в файл readme и измените ссылки.

Конечная точка: `api/top-langs?username=psiyavush`

```md
[![Top Langs](https://github-stats-psiyavushs-projects.vercel.app/api/top-langs/?username=anuraghazra)](https://github.com/psiyavush/github-stats)
```

### Алгоритм статистики языка

Для расчета процентного соотношения языков на языковой карте мы используем следующий алгоритм:

```js
ranking_index = (byte_count ^ size_weight) * (repo_count ^ count_weight)
```

По умолчанию для определения процентных долей языков, показанных на языковой карте (т.е. `size_weight=1` и `count_weight=0`). Однако вы можете использовать параметры `&size_weight=` и `&count_weight=` ля взвешивания расчета использования языка. Значения должны быть положительными действительными числами. 
*   `&size_weight=1&count_weight=0` - (*по умолчанию*) Сортирует по количеству байтов.
*   `&size_weight=0.5&count_weight=0.5` -  (*рекомендуется*) Использует как количество байтов, так и количество репозиториев для ранжирования
*   `&size_weight=0&count_weight=1` - Заказы по количеству репо

```md
![Top Langs](https://github-stats-psiyavushs-projects.vercel.app/api/top-langs/?username=anuraghazra&size_weight=0.5&count_weight=0.5)
```

### Исключить отдельные репозитории

Вы можете использовать этот параметр `&exclude_repo=repo1,repo2` для исключения отдельных репозиториев.

```md
![Top Langs](https://github-stats-psiyavushs-projects.vercel.app/api/top-langs/?username=anuraghazra&exclude_repo=github-readme-stats,psiyavush.github.io)
```

### Скрыть отдельные языки

Вы можете использовать `&hide=language1,language2` чтобы скрыть отдельные языки.

```md
![Top Langs](https://github-stats-psiyavushs-projects.vercel.app/api/top-langs/?username=anuraghazra&hide=javascript,html)
```

### Показать больше языков

Вы можете использоват `&langs_count=` опцию для увеличения или уменьшения количества языков, отображаемых на карте. Допустимые значения — целые числа от 1 до 20 (включительно). По умолчанию установлено значение `5` для `normal` & `donut` и `6` для других макетов.

```md
![Top Langs](https://github-stats-psiyavushs-projects.vercel.app/api/top-langs/?username=anuraghazra&langs_count=8)
```

### Компактный макет языковой карты

Вы можете воспользоваться опцией `&layout=compact` для изменения дизайна карты.

```md
![Top Langs](https://github-stats-psiyavushs-projects.vercel.app/api/top-langs/?username=anuraghazra&layout=compact)
```

### Макет языковой карты «кольцевая диаграмма»

Вы можете воспользоваться опцией `&layout=donut` для изменения дизайна карты.

```md
[![Top Langs](https://github-stats-psiyavushs-projects.vercel.app/api/top-langs/?username=anuraghazra&layout=donut)](https://github.com/psiyavush/github-stats)
```

### Макет языковой карты вертикальной диаграммы Donut

Вы можете воспользоваться опцией `&layout=donut-vertical` для изменения дизайна карты.

```md
[![Top Langs](https://github-stats-psiyavushs-projects.vercel.app/api/top-langs/?username=anuraghazra&layout=donut-vertical)](https://github.com/psiyavush/github-stats)
```

### Макет языковой карты диаграммы пирог

Вы можете воспользоваться опцией `&layout=pie` для изменения дизайна карты.

```md
[![Top Langs](https://github-stats-psiyavushs-projects.vercel.app/api/top-langs/?username=anuraghazra&layout=pie)](https://github.com/psiyavush/github-stats)
```

### Скрыть индикаторы выполнения

Вы можете использовать `&hide_progress=true` чтобы скрыть проценты и индикаторы выполнения (макет будет автоматически установлен на `compact`).

```md
![Top Langs](https://github-stats-psiyavushs-projects.vercel.app/api/top-langs/?username=anuraghazra&hide_progress=true&cache_seconds=86400)
```

### Демо

![Top Langs](https://github-stats-psiyavushs-projects.vercel.app/api/top-langs/?username=anuraghazra&cache_seconds=86400)

*   Компактная планировка

![Top Langs](https://github-stats-psiyavushs-projects.vercel.app/api/top-langs/?username=anuraghazra\&layout=compact)

*   Макет кольцевой диаграммы

[![Top Langs](https://github-stats-psiyavushs-projects.vercel.app/api/top-langs/?username=anuraghazra\&layout=donut&cache_seconds=86400)](https://github.com/psiyavush/github-stats)

*   Вертикальная диаграмма «Пончик»

[![Top Langs](https://github-stats-psiyavushs-projects.vercel.app/api/top-langs/?username=anuraghazra\&layout=donut-vertical&cache_seconds=86400)](https://github.com/psiyavush/github-stats)

*   Макет диаграммы пирог

[![Top Langs](https://github-stats-psiyavushs-projects.vercel.app/api/top-langs/?username=anuraghazra\&layout=pie&cache_seconds=86400)](https://github.com/psiyavush/github-stats)

*   Скрытые индикаторы выполнения

![Top Langs](https://github-stats-psiyavushs-projects.vercel.app/api/top-langs/?username=anuraghazra\&hide_progress=true&cache_seconds=86400)

# Карточка статистики WakaTime

> [!ПРЕДУПРЕЖДЕНИЕ]\
> Обратите внимание, что в настоящее время мы показываем только данные из общедоступных профилей WakaTime. Поэтому вам необходимо убедиться, что **ОБА** `Display code time publicly` и `Display languages, editors, os, categories publicly` включены.

Измените `?username=` на свое имя пользователя [WakaTime](https://wakatime.com)

```md
[![Harlok's WakaTime stats](https://github-stats-psiyavushs-projects.vercel.app/api/wakatime?username=ffflabs)](https://github.com/psiyavush/github-stats)
```

### Демо

![Harlok's WakaTime stats](https://github-stats-psiyavushs-projects.vercel.app/api/wakatime?username=ffflabs&cache_seconds=86400)

![Harlok's WakaTime stats](https://github-stats-psiyavushs-projects.vercel.app/api/wakatime?username=ffflabs\&hide_progress=true&cache_seconds=86400)

*   Компактная планировка

![Harlok's WakaTime stats](https://github-stats-psiyavushs-projects.vercel.app/api/wakatime?username=ffflabs\&layout=compact&cache_seconds=86400)

***

# Все Демо

*   По умолчанию

![Anurag's GitHub stats](https://github-stats-psiyavushs-projects.vercel.app/api?username=anuraghazra&cache_seconds=86400)

*   Скрытие определенной статистики

![Anurag's GitHub stats](https://github-stats-psiyavushs-projects.vercel.app/api?username=anuraghazra\&hide=contribs,issues&cache_seconds=86400)

*   Показ дополнительной статистики

![Anurag's GitHub stats](https://github-stats-psiyavushs-projects.vercel.app/api?username=anuraghazra\&show_icons=true\&show=reviews,discussions_started,discussions_answered,prs_merged,prs_merged_percentage&cache_seconds=86400)

*   Показ значков

![Anurag's GitHub stats](https://github-stats-psiyavushs-projects.vercel.app/api?username=anuraghazra\&hide=issues\&show_icons=true&cache_seconds=86400)

*   Показывает логотип Github вместо уровня рейтинга

![Anurag's GitHub stats](https://github-stats-psiyavushs-projects.vercel.app/api?username=anuraghazra\&rank_icon=github&cache_seconds=86400)

*   Показывает процентиль ранга пользователя вместо уровня ранга

![Anurag's GitHub stats](https://github-stats-psiyavushs-projects.vercel.app/api?username=anuraghazra\&rank_icon=percentile&cache_seconds=86400)

*   Настроить цвет границы

![Anurag's GitHub stats](https://github-stats-psiyavushs-projects.vercel.app/api?username=anuraghazra\&border_color=2e4058&cache_seconds=86400)

*   Включить все коммиты

![Anurag's GitHub stats](https://github-stats-psiyavushs-projects.vercel.app/api?username=anuraghazra\&include_all_commits=true&cache_seconds=86400)

*   Темы

Выберите любую из [тем по умолчанию](#Темы)

![Anurag's GitHub stats](https://github-stats-psiyavushs-projects.vercel.app/api?username=anuraghazra\&show_icons=true\&theme=radical&cache_seconds=86400)

*   Градиент

![Anurag's GitHub stats](https://github-stats-psiyavushs-projects.vercel.app/api?username=anuraghazra\&bg_color=30,e96443,904e95\&title_color=fff\&text_color=fff&cache_seconds=86400)

*   Настройка статистической карты

![Anurag's GitHub stats](https://github-stats-psiyavushs-projects.vercel.app/api/?username=anuraghazra\&show_icons=true\&title_color=fff\&icon_color=79ff97\&text_color=9f9f9f\&bg_color=151515&cache_seconds=86400)

*   Настройка языка карточки

![Anurag's GitHub stats](https://github-stats-psiyavushs-projects.vercel.app/api/?username=anuraghazra\&locale=ru&cache_seconds=86400)

*   Настройка карты конкретного репозитория

![Customized Card](https://github-stats-psiyavushs-projects.vercel.app/api/pin?username=psiyavush\&repo=github-stats\&title_color=fff\&icon_color=f9f9f9\&text_color=9f9f9f\&bg_color=151515&cache_seconds=86400)

*   Карточка GitHub Gists

![Gist Card](https://github-stats-psiyavushs-projects.vercel.app/api/gist?id=bbfce31e0217a3689c8d961a356cb10d&cache_seconds=86400)

*   Настройка карточки GitHub Gists

![Gist Card](https://github-stats-psiyavushs-projects.vercel.app/api/gist?id=bbfce31e0217a3689c8d961a356cb10d&theme=calm&cache_seconds=86400)

*   Популярные языки

![Top Langs](https://github-stats-psiyavushs-projects.vercel.app/api/top-langs/?username=anuraghazra&cache_seconds=86400)

*   Карта WakaTime

![Harlok's WakaTime stats](https://github-stats-psiyavushs-projects.vercel.app/api/wakatime?username=ffflabs&cache_seconds=86400)

***

## Быстрый совет (выровняйте карты)

По умолчанию GitHub не выкладывает карты рядом. Для этого можно использовать такой подход:

```html
<a href="https://github.com/psiyavush/github-stats">
  <img height=200 align="center" src="https://github-stats-psiyavushs-projects.vercel.app/api?username=anuraghazra" />
</a>
<a href="https://github.com/psiyavush/convoychat">
  <img height=200 align="center" src="https://github-stats-psiyavushs-projects.vercel.app/api/top-langs?username=anuraghazra&layout=compact&langs_count=8&card_width=320" />
</a>
```

```html
<a href="https://github.com/psiyavush/github-stats">
  <img align="center" src="https://github-stats-psiyavushs-projects.vercel.app/api/pin/?username=anuraghazra&repo=github-readme-stats" />
</a>
<a href="https://github.com/psiyavush/convoychat">
  <img align="center" src="https://github-stats-psiyavushs-projects.vercel.app/api/pin/?username=anuraghazra&repo=convoychat" />
</a>
```

<details>
<summary>👀 Показать пример</summary>

<a href="https://github.com/psiyavush/github-stats">
  <img height=200 align="center" src="https://github-stats-psiyavushs-projects.vercel.app/api?username=anuraghazra" />
</a>
<a href="https://github.com/psiyavush/github-stats">
  <img height=200 align="center" src="https://github-stats-psiyavushs-projects.vercel.app/api/top-langs?username=anuraghazra&layout=compact&langs_count=8&card_width=320" />
</a>

***

<a href="https://github.com/psiyavush/github-stats">
  <img align="center" src="https://github-stats-psiyavushs-projects.vercel.app/api/pin/?username=anuraghazra&repo=github-readme-stats" />
</a>
<a href="https://github.com/psiyavush/github-stats">
  <img align="center" src="https://github-stats-psiyavushs-projects.vercel.app/api/pin/?username=anuraghazra&repo=convoychat" />
</a>
</details>

# Самостоятельное развертывание проекта

Поскольку API GitHub допускает только 5 тыс. запросов в час, то на  `https://github-stats-psiyavushs-projects.vercel.app/api` возможно, достижения ограничения скорости. Если вы разместите проект на собственном сервере Vercel, то вам не о чем беспокоиться.

<details>
 <summary><b>🛠️ Пошаговое руководство по настройке собственного экземпляра Vercel</b></summary>

1.  Перейдите на [vercel.com](https://vercel.com/).
2.  Нажмите на `Log in`.
    ![](https://camo.githubusercontent.com/360da1819177bece5c252daf28f37ccd2c0b920c77855fbf1e3bee86672c2b20/68747470733a2f2f66696c65732e636174626f782e6d6f652f7063786b33332e706e67)
3.  Войдите в систему GitHub, нажав `Continue with GitHub`.
    ![](https://camo.githubusercontent.com/af53dc07f5231781650a12e2a468f9e99ba36cb10d805f69451b4323efef5040/68747470733a2f2f66696c65732e636174626f782e6d6f652f62396f7865792e706e67)
4.  Войдите в GitHub и разрешите доступ ко всем репозиториям, если будет предложено.
5.  Сделайте форк (Fork) этого репозитория.
6.  Вернитесь на [панель инструментов Vercel](https://vercel.com/dashboard).
7.  Чтобы импортировать проект, нажмите `Add New...` кнопку и выберите нужную `Project` опцию..
    ![](https://camo.githubusercontent.com/a9a9984d0088af1f41c37aca97e38d93f835fb0e2c3d1ec285442fefe09a7d39/68747470733a2f2f66696c65732e636174626f782e6d6f652f336e373666682e706e67)
8.  Нажмите `Continue with GitHub` кнопку, найдите нужный Git Repository и импортируйте его, нажав `Import` кнопку. В качестве альтернативы вы можете импортировать Third-Party Git Repository, используя  `Import Third-Party Git Repository ->` внизу страницы.
    ![](https://camo.githubusercontent.com/37f4e2f28d6eb87c9a9c269989b1c36352490e2a5aa787361ae4f0d4ab512810/68747470733a2f2f66696c65732e636174626f782e6d6f652f6d67357030342e706e67)
9.  Создайте [здесь](https://github.com/settings/tokens/new) персональный токен доступа (PAT) и включите разрешения `repo` и`user` (это позволит отображать статистику из приватных репозиториев и статистику пользователей).
10. Добавьте PAT как переменную среды с именем `PAT_1` (как показано).
    ![](https://camo.githubusercontent.com/6e94bad8da34de7d718ecc42bbbbc221af46435439450982fc2e74ab503ca1e8/68747470733a2f2f66696c65732e636174626f782e6d6f652f3079636c696f2e706e67)
11. Нажмите «Deploy», и все готово. Посмотрите свои домены, чтобы использовать API!

</details>

## Отключить защиту ограничения скорости

Github Stats содержит несколько переменных среды Vercel, которые можно использовать для снятия защиты от ограничения скорости:

*   `CACHE_SECONDS`: Эта переменная среды имеет приоритет над минимальными и максимальными значениями нашего кэша и может обойти эти значения для размещенных на собственном сервере экземпляров Vercel.

Инструкции по добавлению этих переменных среды в экземпляр Vercel см  [в документации Vercel .](https://vercel.com/docs/concepts/projects/environment-variables)

## Поддерживайте актуальность своего fork

Вы можете поддерживать свой форк, а значит и свой частный экземпляр Vercel в актуальном состоянии с помощью [кнопки GitHub Sync Fork](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/syncing-a-fork).