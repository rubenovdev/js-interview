## Вопросы по JavaScript

### Типы данных
<a name="types" href="#types">Какие типы данных существуют в JavaScript?</a>
Расскажи все, что знаешь о типах данных

Сколько типов данных в JavaScript?

как происходит преобразование строки в число

Сколько типов данных, что делает Symbol
На какие категории можно разделить типы в JavaScript?

Сколько типов данных в JavaScript ? Назови типы данных ? В чем разница между примитивными и не примитивными данными ?

В чем отличие null и undefined ?

Что такое простые типы? Чем они отличаются от объектов?

-
Ответ
В отличие от объектов, примитивные типы иммутабельны (например, при конкатенации двух строк создается новая).
При копировании, примитивные типы копируются по значению, а объекты - по ссылке.
Объекты хранятся в куче (Heap), а примитивы - в стеке (Stack).
Также стоит отметить, что для всех примитивных типов есть свои объектные обертки.

-



### Переменные
В чем разница между var, let и const?
Какая разница между var, let, const

Что такое хостинг переменных в JavaScript?


### Сетевые запросы
Что такое CORS? В чем его суть? Ты знаком с CORS? Что это?

Как работают методы GET и POST и в чем их разница? Как работает протокол HTTP, как происходит отправка запросов к серверу?

Что такое JSON и для чего он нужен?

Расскажи про GET/POST запросы, что они делают, где и как используются и в чем их различие?

Сколько файлов могут подгружаться на страницу параллельно ? В чем разница между HTTP/1 и HTTP/2 ?

как работают разные сетевые протоколы (IP, TCP, HTTP/S/2, UDP, RTC, DNS, и так далее).

xhr, fetch

Состав запроса: заголовки, метод, URL, response

Разница между GET, POST, PUT, DELETE

Разница между http, http2.0, https (SSL шифрование)

Основные способы взаимодействия frontend -> backend. Какие существуют способы отправки данных?  (Обязательно)
Ограничения XmlHttpRequest? Как CORS и JSONP снимают эти ограничения?

WebSocket
REST
JSON:API

что такое user-agent, json web token

как на фронте принять и обработать файл от сервера (а не строку)

с помощью каких протоколов можно осуществлять запросы от клиента к браузеру

Из чего состоит HTTP-запрос?


### this, call, apply, bind
Расскажи про this. Что такое this?

Что такое this ? Как оно работает, от чего зависит ?

Расскажи про bind, call, apply

### Замыкание
Что такое замыкания? Покажи пример замыкания в js
Что такое замыкание в js ? Что такое лексическое окружение ?
Что такое замыкания в JavaScript? Приведи пример?
Объясните своими словами, что такое замыкание?

Как создать функцию, не являющуюся замыканием?
Ответ: никак

В прошлом в JavaScript не было лексического окружения на уровне блоков кода. предположи как разработчики рашали эту проблему (ответ: IIFE)


### Хранение данных в браузере
Что такое Local Storage и как оно работает?
Как работают кэш и куки в браузере и с JavaScript?
Перед тобой стоит задача сохранять данные из инпутов на стороне клиента, как ты ее реализуешь ? Что такое кэш, куки, local storage
local storage ,  session storag

### Объекты
Что относится к объектам (Map, Set, Promise)

что делают for in , for of

как перебрать свойства объектов, какие свойства не будут видны при переборе for in (дескрипторы)

Что такое Map, Set, WeakMap, WeakSet

что делает Метод Object.freeze()


### Строки и их методы
Расскажи про строки в JavaScript, в какой кодировке они хранятся, сколько бит отводится на хранение одного символа, какие методы они имеют, как сделать поиск по строке?


### Массивы и их методы
Что делает метод reduce? Какие методы массивов ты знаешь? Назови все, которые знаешь

в чем разница между Разница между map и forEach


### Операторы сравнения
В чем отличие === от == ? Какой используете вы и почему?


### DOM, события
Что делает event.stopPropagation() и event.preventDefault()?
Как можно остановить выполнение Event

Как создать/вставить/удалить элемент из DOM?

Какими способами можно взять элемент из DOM?

Что делает метод document.write?

Что такое делегирование событий? У тебя есть таблица 500 на 500, и нужно взаимодействовать с каждой ячейкой, как это лучше сделать?

что такое Всплытие и погружение

в чем разница между target и currentTarget


### Асинхронное программирование, промисы, promise, async/await
Расскажи все о промисах ? Как работают асинхронщина в js ? Как еще можно вызвать асинхронный код ? Что такое Event Loop, как отрабатывают асинхронные действия в js ?

Расскажи про Event Loop

Что ты знаешь о синхронных и ассинхронных функциях в JavaScript, Async/Await?

Расскажи про микрозадачи и макрозадачи

Вопрос со звездочкой(*) В чем разница между .then(f1, f2) и .then(f1).catch(f2) ?

Расскажи про setTimeout и setInterval? сколько аргументов может принимать setTimeout и куда они передаются если их больше 2

Почему нулевая задержка в setTimeout не гарантирует мгновенного запуска задачи?
ответ: Любая задержка в setTimeout не гарантирует, что callback начнет выполняться через это значение. Стоит рассматривать это значение как минимальную возможную задержку, запуск задачи начнется когда наступит её очередь.

Сколько потоков браузер выделяет одной вкладке с выполняющимся JavaScript’ом?

Какими методами можно прервать цепочку промисов не прибегая к .then/.catch? (никакими, ее нельзя прервать)

Что такое web worker, для чего нужен, как работает

Что такое генераторы, как работают, для чего нужны

что такое промис, какое api есть (resolve, reject, all, race)

как работает async await , как вызвать несколько await (promise.all)

расскажи про генераторы, что делает ключевое слово yield, что такое итератор

async await, Promise , зачем нужны

Можно ли менять then и catch местами? Эквивалентны ли записи?
```
p.then(() => console.log(1))
 .catch(() => console.log(2));
  
p.catch(() => console.log(2))
 .then(() => console.log(1));
```

Как перевести промис, возвращаемый методом catch в состояние rejected?


### Конструкторы, создание объектов через "new"
Что такое конструкторы в js ? Что происходит, когда мы создаем объект через new ?


### Прототипы, наследование
Как работает прототипное наследование в js ?
Расскажи про прототипирование, наследование. Как оно работает в JS? На что ссылка Object в прото?
Как работают прототипы в js ?

proto и prototype в чем разница

На что ссылка Object в прото?

Что происходит при обращении к свойству объекта?
Как создать новый объект, прототипом которого является существующий?
Как проверить является ли свойство собственным, либо найдено в цепочке прототипов?
Как унаследовать одну функцию от другой? Почему не подходят Object.create и функция-конструктор? Зачем это может потребоваться?

Обычно `Foo.prototype !== Foo.__proto__`, где Foo - произвольная функция. Объясните, почему `Function.prototype === Function.__proto__` ?


### Классы
Что такое классы в js ? Чем они отличаются от функций ? Это что-то принципиально новое ? Как классы работают с наследованием ? Что делает extends

Расскажи что знаешь о классах в JavaScript?

классы, static методы

Что такое классы, их API, для чего были созданы
Что делает конструктор ?


### Функции
Что такое function в JavaScript?
Ответ: Просто: функция имеет отдельный тип "function" и используется в целях разделения, переиспользования функциональности. Сложно: функция в JavaScript на самом деле является подтипом object и имеет внутреннее свойство [[Call]] благодаря которому появляется возможность вызова.

Как задать дефолтное значение аргументу функции ?

Function Expression в сравнении с Function Declaration

Что делает функция eval(code)?
Что делает eval ?

Чем стрелочная функция отличается от обычной?
разница между arrow function и function declaration
особенности arrow fn и вызова через new


### Алгоритмы и структуры данных
Знаком ли ты с алгоритмическими основами?

Назови разницу между структурами данных: очередь и стек

что такое хэш таблица

метод линейного пробования и квадратичного



### Тестирование, тесты
Тестируешь ли ты свой код перед тем, как залить на prod, как ты его тестируешь?

какой методологией пользуешься ?

### Общие
Где обучаешься? Из каких источников берешь информацию, что читаешь, сколько времени уделяешь своему обучению?

Почему ты хочешь к нам на стажировку? Какова твоя мотивация?

Почему хочешь на стажировку? Почему именно МТС? Чего ожидаешь от стажировки?

Расскажите о вашем опыте разработки. расскажите о своих должностных обязанностях. Доводилось ли вам работать в команде? В каких ОС вы работали?

Расскажи вкратце о себе, чем занимаешься последние два года (связанное с разработкой)?

Расскажи про проекты, которыми занимаешься/занимался. Что самое сложное ты реализовал? Самая интересная задача?

Расскажи о проектах, в которых ты участвовал, о своих проектах?

расскажи про самую интересную задачу, которую делал

Расскажи о своем опыте работы? Над чем работаешь, с какими технологиями?

Чем занимаешься в свободное время?
Как развиваешься, где обучаешься в свободное время?
Почему решил уйти с текущего места?

### Общие технические
Работал ли ты с фреймворками? Что больше нравится React или Vue?
Использовал ли ты в своих проектах фреймворки? Знаком ли ты с фреймворками?
В чем разница между React и Vue? На чем тебе больше нравится работать? Знаком с Angular? В чем разница между фреймворком и библиотекой? Есть ли разница в работе с данными на React и Vue?

Работал ли с Node.js? Настраивал backend?

Работал ли ты с backend-частью? (желательно наличие опыта в backend разработке)

Почему ты выбрал именно Frontend, почему не Backend?

Ты работаешь в офисе в Москве и сделал красную кнопку, а тестировщик, который работает на удаленке из Владивостока, получил на тестирование твой год, посмотрел и говорит, что кнопка синяя. Предположи, почему так и что ты будешь делать в такой ситуации ?

В чем отличия ES5 от ES6?

Какими нововведениями из ES6 ты пользуешься? Какие нравятся? Какие знаешь?

Объясни что такое база данных одним предложением

Назови паттерны программирования

Назови три основные принципа ООП

Чем функциональное программирование отличается от объектно-ориентированного

что такое PWA


### методологии разработки
Какие методы управления проектами используете? Как получаешь задачи, от кого? Знаешь о Scrum?

Какие принципы Scrum ты используешь/знаешь

Какие есть основные ценности Kanban?




### Без темы
Какие мертвые зоны в JavaScript знаешь ?

Что такое утечка памяти в js, приведи примеры
что такое утечка памяти и как ее устранить

Что такое proxy объект

Различия монолитных и атомарных SPA



# React
Расскажи про жизненный цикл компонента в React
Жизненный цикл компонента

Какие замены есть в stateless компонентах (дид кетч)

Хуки, в основном setState, useEffect

Разница вызова setState через объект и стрелочную функцию

В чем отличие функциональных компонентов от классовых?

Назови методы жизненного цикла классового компонента ? Чем отличаются классовые компоненты от функциональных ? Расскажи, что делают хуки useState и useEffect ? Что передается вторым аргументом в useEffect ? Что передается в useState ?

Чем функциональные компоненты отличаются от классов? Есть ли разница в оптимизации?

В чем разница между state и store

Для чего в React нужен key

Что такое виртуальный DOM, для чего он нужен и что из себя представляет в JavaScript

Какими способами можно оптимизировать компонент

Разница между Pure Component и Component
Оптимизация компонента

Паттерны React-компонентов, HOC

Context


# Redux
Что такое Reducer, что делает, что такое чистая функция, можно ли в ней делать fetch-запрос или другой side-эффект

Весь флоу: store, action, reducer, dispatch, provider, connect (mapStatetoprops, mapDispatchprops, можно и mergeProps добавить, options)

Как происходит связь между store и компонентом

работа с асинхронными экшенами
Это либо redux-thunk, там все просто понятно, либо redux-saga


# HTML/CSS
Чем отличаются блочные, инлайновые и инлайново-блочные элементы?

Расскажи про flexbox. Где уместно использовать? Какие параметры имеют флексы?

Расскажи про grid. Где уместно использовать? Какие параметры имеют гриды?

Чем абсолютное позиционирование отличается от фиксированного?

Что такое БЭМ? Чем элементы отличаются от блоков? В чем суть БЭМ’а?

Работал ли ты с препроцессорами? Зачем они нужны?

На чем ты обычно делаешь сетку сайта ? Что знаешь о флексах ? Как выровнять элемент по центру с помощью flex ? Как изменить позиционирование элементов, чтобы они отобразились по вертикали ?

Рендеринг страницы: что такое reflow и repaint

Какие значения свойства display ты знаешь?

Что делает тег <script> и какие атрибуты этого тега ты знаешь? async и defer
  
Работал ли с iframe?

В чем разница между HTML5 и HTML4

Атрибут prefetch, preload, autofocus

Особенности различных браузеров (IE10+)
Вам нужно понять, почему страница отображается некорректно в Safari на iOS и в IE на Windows 7. Ваши действия?

От чего считаются проценты, если написать `padding-top: 50%`?

Чем отличается display: none от visibility: hidden?

Какие виды позиционирования Вы знаете? (новый вид sticky) В чем отличие static от relative?

Как нужно и можно оптимизировать изображения для фронтенда?

Как расположить блоки по горизонтали?

какие css -свойства труднее всего рендерить браузеру


# проектирование веб-приложений
Как реализовать авто-логаут по причине бездействия пользователя n-минут? Если приложение открыто в нескольких вкладках?

Как реализовать регистрацию/авторизацию пользователя?

как можно обеспечить offline работу приложения

какие есть способы сделать приложение доступным


# Тесты
Пишите ли вы тесты? Если да, то какие?
Каким критериям должен удовлетворять unit-тест?
В чем суть методики TDD?
Знакома ли вам методология BDD? Приходилось ли использовать, если да, то в каких случаях?


# Node.js / NPM
Необходимо узнать последнюю версию npm-пакета. Ваши действия?
package.json: devDependencies, dependencies, peerDependencies
Для чего нужны npm scoped packages?
Что делает команда npm ci?

