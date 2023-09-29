# Проектная работа по курсу OTUS HTML/CSS

## Описание работы

Вёрстка проекта выполнена по макету ([макет](https://www.figma.com/file/IsT8OAe334nd2nwc9pKCu8/Otus-mocks-2023-08-10?type=design&node-id=9591%3A3&mode=design&t=e7XUyL7rQYgbnGEt-1)) с применением desktop-first подхода и адаптацией для планшета и мобильных устройств. В ветках bootstrap и tailwind верстка выполнена с применением соответствующих ui-библиотек.
Сборка проекта выполняется сборщиком Webpack. Описание скриптов в разделе ["Скрипты для сборки проекта"](#скрипты-для-сборки-проекта).
Деплой выполняется с помощью npm пакета [gh-pages](https://www.npmjs.com/package/gh-pages)


## Скрипты для сборки проекта

Запуск продакшн сборки webpack и запуск локального http-server:
```
npm start
```
 Запуск dev-сборки webpack:
```
npm run build
```
  Запуск продакшн сборки webpack:
```
npm run prod
```
 Запуск dev-сервера webpack на продакшн-сборке:
```
npm run server
```
 Деплой продакшн-сборки на github-pages: [otus-css-novitskiy](https://v-nvtsk.github.io/otus-css-novitskiy/ "Link to deployed page on github-pages"):
```
npm run deploy
```

## Lighthouse results
Основная проблема в Cumulative Layout shift.
### Desktop
![Alt text](./lighthouse/LH-desktop.png)

### Mobile
![Alt text](./lighthouse/LH-mobile.png)

## Содержание курса и домашних заданий

### [1 Введение в Web](https://otus.ru/learning/234741//#)

#### Краткое содержание

1. организационные вопросы  
2. история WWW. зачем изобрели Web.  
3. изучаемые на курсе технологии  
4. инструменты  
    - фигма  
    - редактор кода на примере VSCode  
    - онлайн-редактор кода  
    - инспектор кода в браузере

### [2 Version Control](https://otus.ru/learning/234741//#)

#### Цели занятия
Научиться работать с системой контроля версий Git. Работа в GitHub
#### Краткое содержание

Что такое и на чем основано версионирование?  
Как установить и настроить гит на разные ОС  
Терминал в VSCode  
Локальная работа с изменениями через терминал (git add, git status, git commit, git branch, git checkout)  
Использование встроенных возможностей редактора для работы с гит вместо терминала  
Регистрация и создание репозитория на GitHub  
Работа с удаленным и локальным репозиториями  
Плагины и клиенты (GitHub desktop) для помощи в работе
#### Домашнее задание

1.  Установить git, произвести базовую настройку.
2.  Зарегистрироваться на GitHub. Создать репозиторий c названием по шаблону otus-css-surname. Именно так!
3.  Клонировать репозиторий, добавить пустой файл index.html, а так же создать README.md и научиться его редактировать.
4.  Сделать commit в ветку master (может называться main).
5.  Сделать push.
6.  Убедиться, что изменения успешно перенесены на удаленный репозиторий.
7.  В качестве выполненного ДЗ прикрепить ссылку на репозиторий.
8.  Изучить дополнительные материалы
### [3 Почему html - это не язык программирования](https://otus.ru/learning/234741//#)

#### Цели занятия

создать первую html страницу

#### Краткое содержание

1. HTML - всего лишь формат текстового файла.  
    - способы создания HTML страниц  
    - инструменты работы  
    - текстовый редактор VSCode  
    - CodeSandbox, CodePen  
2. как форматировать текст для веб страницы  
    - почему lorem ipsun - не всегда хорошая идея;  
3. введение в семантическую разметку, MDN  
    -особенности SEO оптимизации  
    - особенности a11y  
    - особенности разметки с дизайном  
4. упражнение на разметку  
5. нюансы разметки  
#### Домашнее задание

1.  Создайте новую ветку от основной (main или master), например, semantics
2.  Перейдите по ссылке [https://www.figma.com/file/WZBpyrcVpI1edxPzIHCg1E/Otus-mocks](https://www.figma.com/file/WZBpyrcVpI1edxPzIHCg1E/Otus-mocks "https://www.figma.com/file/WZBpyrcVpI1edxPzIHCg1E/Otus-mocks")
3.  Изучите макет.
4.  Определите, какие по вашему, изученные ранее структурные теги (header, nav, section, main, aside article, footer) надо использовать. Добавьте семантические теги для элементов страницы и текста. Стилизовать, позиционировать и т.д. элементы не нужно. Исключительно семантика. Только HTML.
5.  Перенесите текст, заголовки, списки, цитаты и т.п. с макета в код. Используйте соответствующие теги.
6.  Добавьте картинки в код используя тег img. Можно экспортировать из макета и положить в папку img. Фото - форматом jpg, иконки - svg.
7.  Будет здорово, если каждый блок вы сможете отделить соответствующими комментариями, для удобства чтения.
8.  Делаем тематические коммит-сообщения, например, git commit -m “Added html semantic structure”. Пушим.
9.  Создайте pull request текущей ветки в основную (main или master).
10.  Скиньте ссылку на данный pull request. Ссылка должна быть вида: что-то/pulls/число
  
### [4 CSS: история стилей](https://otus.ru/learning/234741//#)

#### Краткое содержание

1. три вида написания CSS  
    - Inline  
    - Style tag  
    - CSS file  
2. User Agent CSS  
3. как происходит рендеринг HTML страницы  
     - Render Tree  

### [5 Типографика](https://otus.ru/learning/234741//#)

#### Краткое содержание

узнать что такое типографика  
научиться подключать шрифты по ссылке и локально  
базовая работа со шрифтами:  
    - стилевые приемы  
    - единицы измерения (px, em, rem, vh, vw, %, функция calc)  
    - оптимизация шрифтов
#### Домашнее задание

1.  Создайте новую ветку от основной (main или master), например, typography
2.  Перейти по ссылке на Figma макет - [https://www.figma.com/file/WZBpyrcVpI1edxPzIHCg1E/Otus-mocks](https://www.figma.com/file/WZBpyrcVpI1edxPzIHCg1E/Otus-mocks "https://www.figma.com/file/WZBpyrcVpI1edxPzIHCg1E/Otus-mocks").
3.  Изучаем макет. Какие шрифты и их варианты используются? Можно использовать плагин Font Master или Font Fascia к Figma.
4.  Подключить необходимые шрифты. Через сервис fonts Google и локально.
5.  Задать странице основной шрифт, базовый размер и высоту строки.
6.  Для каждого текстового элемента задать текстовые свойства по макету.
7.  Коммитим, пушим.
8.  Делаем pull request. Присылаем ссылку на него.

### [6 Box model в деталях](https://otus.ru/learning/234741//#)

#### Краткое содержание

box model в деталях, display, box sizing, универсальный селектор \*,  
Свойство background
#### Домашнее задание

1.  Создайте новую ветку от основной (main или master), например, hero-section
2.  Перейти по ссылке на Figma макет - [https://www.figma.com/file/WZBpyrcVpI1edxPzIHCg1E/Otus-mocks](https://www.figma.com/file/WZBpyrcVpI1edxPzIHCg1E/Otus-mocks "https://www.figma.com/file/WZBpyrcVpI1edxPzIHCg1E/Otus-mocks").
3.  Изучаем макет, стараемся его «прочитать». Какой сайт будет в ширину? Как будет тянуться или сжиматься? Что из себя представляют секции? Цель не фиксированный, а «резиновый» сайт. Подумайте, какие ширины можно задать в процентах, а какие останутся фиксированными. Отступы на данный момент лучше задать фиксированными.
4.  Необходимо сверстать меню и первую секцию. Для фона секции используйте фоновую картинку, она должна быть от края до края барузера.
5.  Сделать коммиты, пуш. Делаем тематические коммит-сообщения, например, git commit -m “style: add styling for hero section”
6.  Делаем pull request. Присылаем ссылку на него.

### [7 Позиционирование элементов в деталях](https://otus.ru/learning/234741//#)

#### Краткое содержание

свойство position: relative, absolute, fixed, sticky и координатные свойства,  
как центрировать элемент с помощью position и transform,  
зачем нужны CSS resets,  
как добавлять фоновое изображение

### [9 Selector priority](https://otus.ru/learning/234741//#)

#### Краткое содержание

\- специфичность и приоритеты правил  
\- ключевое слово !important  
\- значение inherit

### [10 Layout: введение, основы](https://otus.ru/learning/234741//#)

#### Краткое содержание

как исторически менялись подходы: таблицы, инлайн-блоки, флоаты и современные технологии. Модульная сетка,  
основные виды layouts в дизайне, как понимать что имел в виду дизайнер,  
как один и тот же layout можно сделать многими способами,  
верстка PixelPerfect - за и против

### [11 Flexbox layout](https://otus.ru/learning/234741//#)

#### Краткое содержание

все о flexbox layout.
#### Домашнее задание

Использование flex для оформления секции Biography

1.  Создайте новую ветку от основной (main или master), например biography-section
2.  В соответствии с макетом: [https://www.figma.com/file/WZBpyrcVpI1edxPzIHCg1E/Otus-mocks](https://www.figma.com/file/WZBpyrcVpI1edxPzIHCg1E/Otus-mocks "https://www.figma.com/file/WZBpyrcVpI1edxPzIHCg1E/Otus-mocks") верстаем следующую секцию Biography, используя flex для расположения элементов.
3.  Проверить расположение элементов по PixelPerfect. Проверяем как ведёт себя контент при разных размерах окна браузера - нет горизонтального скролла, колонки резиновые и тянутся при уменьшении ширины страницы.
4.  Делаем коммиты и пуш. Создаём pull request и присылаем ссылку на него


### [12 Grid layout](https://otus.ru/learning/234741//#)

#### Краткое содержание

все о grid layout.
#### Домашнее задание

Применение grid для оформления секции Testimonials

1.  Создайте новую ветку от основной (main или master), например, testimonials-section
2.  В соответствии с макетом: [https://www.figma.com/file/WZBpyrcVpI1edxPzIHCg1E/Otus-mocks](https://www.figma.com/file/WZBpyrcVpI1edxPzIHCg1E/Otus-mocks "https://www.figma.com/file/WZBpyrcVpI1edxPzIHCg1E/Otus-mocks") верстаем следующую секцию Testimonials
3.  Проверить расположение элементов по PixelPerfect. Проверяем как ведёт себя контент при разных размерах окна браузера - нет горизонтального скролла, колонки резиновые и тянутся при уменьшении ширины страницы.
4.  Сама секция является grid-контейнером сетки. При необходимости добавляем div'ы для организации ячеек, оформляем контент в ячейках
5.  Делаем коммиты и пуш. Создаём pull request и присылаем ссылку на него

### [13 Workshop по сеткам](https://otus.ru/learning/234741//#)

#### Краткое содержание

на этом исключительно практическом занятии вам предстоит решить несколько задач по расположению элементов, научиться применять и выбирать подходящие для этого технологии (флексы или гриды)  
#### Домашнее задание

1.  Создайте новую ветку от основной (main или master), например designers-section
2.  В соответствии с макетом: [https://www.figma.com/file/WZBpyrcVpI1edxPzIHCg1E/Otus-mocks](https://www.figma.com/file/WZBpyrcVpI1edxPzIHCg1E/Otus-mocks "https://www.figma.com/file/WZBpyrcVpI1edxPzIHCg1E/Otus-mocks") верстаем секцию Designers.
3.  Проверить расположение элементов по PixelPerfect. Проверяем как ведёт себя контент при разных размерах окна браузера - нет горизонтального скролла, колонки резиновые и тянутся при уменьшении ширины страницы.
4.  Исходим из того, что у нас множество из любого количества дизайнеров. И дизайнер с крупной картинкой может находится на любом месте. При этом предусмотреть поведение, если дизайнеров будет больше.
5.  Делаем коммиты и пуш. Создаём pull request и присылаем ссылку на него. В комментарии к заданию обоснуйте выбранный вами подход к расположению элементов

### [5 Поддержка браузеров, новые технологии и fallbacks](https://otus.ru/learning/234741//#)

#### Краткое содержание

что такое и зачем нужны fallbacks:  
\- совместимость браузеров с современными CSS технологиями. Сервис caniuse  
\- новые технологии, к которым уже пора присмотреться  
@supports  
вендорные префиксы и автопрефиксер
#### Домашнее задание

1.  Создайте новую ветку от основной (main или master), например, strong-points-section
2.  В соответствии с макетом: [https://www.figma.com/file/WZBpyrcVpI1edxPzIHCg1E/Otus-mocks](https://www.figma.com/file/WZBpyrcVpI1edxPzIHCg1E/Otus-mocks "https://www.figma.com/file/WZBpyrcVpI1edxPzIHCg1E/Otus-mocks") верстаем следующую секцию Strong points с учетом поддержки браузеров
3.  Проверить расположение элементов по PixelPerfect. Проверяем как ведёт себя контент при разных размерах окна браузера - нет горизонтального скролла, колонки резиновые и тянутся при уменьшении ширины страницы.
4.  Делаем коммиты и пуш. Создаём pull request и присылаем ссылку на него. В комментарии к заданию обоснуйте выбранный вами подход к расположению элементов.

### [16 Введение в media queries](https://otus.ru/learning/234741//#)

#### Краткое содержание

1\. Media queries  
\- как правильно писать media-rules  
\- как применять media-feature  
\- как правильно тестировать media queries с browserstack, xcode, android studio.  
2\. единицы размера вьюпорта  
3\. классические breakpoints  
4\. резиновая, адаптивная и отзывчивая верстка

### [17 Mobile-first vs desktop-first](https://otus.ru/learning/234741//#)
#### Краткое содержание

подходы mobile-first vs desktop-first,  
организация css-кода,  
тестирование верстки

#### Домашнее задание

Адаптивная верстка макета
1.  Работу ведем в соответствующей ветке. Например, mobile-development.
2.  Необходимо адаптировать макет для планшетного и мобильного вида. Выбрать либо mobile-first, либо desktop-first подход и обосновать выбор в сообщении к работе. Убедитесь в том, что на всем сайте не появляется горизонтальной прокрутки, только на отдельных секциях, где это было задумано дизайнером. Скрывать прокрутку свойствами css нельзя.
3.  Сделать коммит, пуш. Прислать ссылку на ПР.


### [18 Анимации CSS](https://otus.ru/learning/234741//#)

#### Краткое содержание

1\. Render tree, отличие компоновки от отрисовки, какие свойства к ним относятся  
2\. как создавать анимации, как их оптимизировать  

#### Домашнее задание

1.  Работу ведем в соответствующей ветке. Например, animation.
2.  Необходимо добавить интерактивным элементам (ссылкам) простые плавные анимации по наведению и фокусу.  
    Дополнительно: сделать анимацию по наведению на изображения в одной из секций, на ваш выбор.
3.  Сделать коммит, пуш. Прислать ссылку на ПР.

### [19 Особенности мобильной верстки](https://otus.ru/learning/234741//#)

#### Краткое содержание

CSS для мобильных браузеров  
1\. верстка мобильного меню  
2\. Нюансы мобильного css  
3\. Оптимизация  
\- Шрифтов (вариативные, display: swap)  
\- Графики (picture)

### [20 Номенклатура](https://otus.ru/learning/234741//#)

#### Краткое содержание

что такое CSSOM;  
методологии BEM, Atomic CSS и другие.

#### Домашнее задание

1.  Работу ведем в соответствующей ветке. Например, bem.
2.  Провести рефакторинг кода: используя BEM номенклатуру, разделить CSS-код на правильно названные субмодули;
3.  Сделать коммит, пуш. Прислать ссылку на репозиторий.

### [21 Bootstrap](https://otus.ru/learning/234741//#)
#### Краткое содержание

Bootstrap.

#### Домашнее задание

Описание/Пошаговая инструкция выполнения домашнего задания:

1.  Работу ведем в соответствующей ветке. Например, bootstrap.
2.  Необходимо переделать макет на Bootstrap.
3.  Сделать коммит, пуш. Прислать ссылку на ПР. Мержить изменения в основную ветку не обязательно, укажите о Bootstrap-версии в файле readme.md

### [22 Tailwind](https://otus.ru/learning/234741//#)

#### Краткое содержание

Tailwind.
#### Домашнее задание

Tailwind

Цель:

В этом ДЗ вы разработаете макет.

Описание/Пошаговая инструкция выполнения домашнего задания:

1.  Работу ведем в соответствующей ветке. Например, tailwind.
2.  Необходимо подключить Tailwind и сделать макет с его использованием, заменив БЭМ-классы на tailwind-классы.
3.  Сделать коммит, пуш. Прислать ссылку на ПР. Мержить изменения в основную ветку не обязательно, укажите о Tailwind-версии в файле readme.md

### [23 Введение в JavaScript](https://otus.ru/learning/234741//#)

#### Краткое содержание

как называть переменные и функции  
что такое объекты  
как работать с DOM  
решение простых задач  

### [25 Настройка окружения для верстки](https://otus.ru/learning/234741//#)
#### Краткое содержание

изучить основные принципы работы с терминалом:  
1\. терминал в VS Code  
\- навигация внутри терминала  
\- установка npm и node  
2\. как использовать npm  
3\. как заменить плагины на пакеты (на примере сервера)

#### Домашнее задание

Настройка окружения

Цель:

Установить Node JS, научится устанавливать пакеты для проекта

Описание/Пошаговая инструкция выполнения домашнего задания:

1.  Работу ведем в соответствующей ветке. Например, packages
2.  Установить npm-пакеты http-server, prettier, lodash, убедиться в изменении файла package.json
3.  Сделать коммит, пуш. Прислать ссылку на ПР.

### [26 Установка Webpack](https://otus.ru/learning/234741//#)

#### Цели занятия

Создать минимальную конфигурацию Webpack 5

#### Краткое содержание

настройка Webpack для работы с HTML/CSS, регулярные выражения, работа с картинками и шрифтами

### [27 Автоматизация процессов](https://otus.ru/learning/234741//#)

#### Краткое содержание

настроить автоматизацию сборки,  
познакомиться с препроцессором SASS
#### Домашнее задание

Webpack

Цель:

Научиться автоматизировать процессы с помощью Webpack

Описание/Пошаговая инструкция выполнения домашнего задания:

1.  Работу ведем в соответствующей ветке. Например, automatization.
2.  Настроить файлы конфигурации Webpack для разработки (дополнительно: и продакшена) проекта
3.  Проверить корректность файла .gitignore
4.  Сделать коммит, пуш. Прислать ссылку на ПР.

### [28 Оптимизация ассетов](https://otus.ru/learning/234741//#)
#### Краткое содержание

минификация CSS, JS файлов для проекта;  
хеширование файлов;  
оптимизация изображений, шрифтов.


#### Домашнее задание

Оптимизация ассетов

Цель:

Научиться оптимизировать графику, шрифты, минимизировать стили и js-код

1.  Работу ведем в соответствующей ветке. Например, optimization.
2.  Настроить минификацию CSS/JS на проекте, оптимизировать изображения, шрифты
3.  Сделать коммит, пуш. Прислать ссылку на ПР.

### [29 Деплой страницы](https://otus.ru/learning/234741//#)

#### Краткое содержание

деплой веб-сайта с помощью GitHub Pages

#### Домашнее задание

Деплой проекта
Описание/Пошаговая инструкция выполнения домашнего задания:

1.  Смержить все итоговые изменения в master/main репозитория на GitHub
2.  Опубликовать проект на GitHub Pages
3.  Прислать ссылки на репозиторий и опубликованную версию проекта


### [30 Аналитика и поддержка](https://otus.ru/learning/234741//#)

#### Краткое содержание

как проверить производительность сайта;  
как узнать статистику сайта;  
как использовать Lighthouse для аналитики страницы

#### Домашнее задание

Аналитика и поддержка

Цель:
В этом ДЗ вы разместите счетчик статистики вашей работы и проверите показатели качества вашего сайта

1.  Работу ведем в соответствующей ветке. Например, support.
2.  Добавить счетчик от Google Analytics/Я.Метрика для страницы
3.  Проверить страницу с помощью Google Lighthouse, добавить данные о качестве в Readme.md
4.  Сделать коммит, пуш. Прислать ссылки на репозиторий и опубликованную версию проекта

### [32 Выбор темы и организация проектной работы](https://otus.ru/learning/234741//#)
#### Краткое содержание

правила работы над проектом и специфика проведения итоговой защиты;  
требования к результату проекта и итоговой документации.

#### Проект

Проектная работа

Цель:

В этом ДЗ необходимо утвердить в чате по ДЗ тему проекта (для всех - Mod studio), разработать презентацию о личных итогах курса, презентовать проект и прислать ссылку на задеплоенную итоговую версию. В файле readme.md должна быть вся информация о проекте: как запустить сборку, есть ли ветки с отдельными фичами, что не задеплоены в мастер.

Описание/Пошаговая инструкция выполнения домашнего задания:

1.  Отправить тему Mod studio
2.  Прислать презентацию личных итогов курса
3.  Прислать ссылку на задеплоенную итоговую версию
