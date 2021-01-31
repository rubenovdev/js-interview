# js-interview


# JS
### Типы данных
Какие типы данных существуют в JavaScript?

Расскажи все, что знаешь о типах данных

### Сетевые запросы
Что такое CORS? В чем его суть?

### this, call, apply, bind
Расскажи про this. Что такое this?

Что такое this ? Как оно работает, от чего зависит ?

Расскажи про bind, call, apply

### Замыкание
Что такое замыкания? Покажи пример замыкания в js
Что такое замыкание в js ? Что такое лексическое окружение ?


### Массивы и их методы
Что делает метод reduce? Какие методы массивов ты знаешь? Назови все, которые знаешь


### Операторы сравнения
В чем отличие === от == ?


### DOM, события
Что делает event.stopPropagation() и event.preventDefault()?


### Асинхронное программирование, промисы, promise, async/await
Расскажи все о промисах ? Как работают асинхронщина в js ? Как еще можно вызвать асинхронный код ? Что такое Event Loop, как отрабатывают асинхронные действия в js ?

Расскажи про микрозадачи и макрозадачи

Вопрос со звездочкой(*) В чем разница между .then(f1, f2) и .then(f1).catch(f2) ?


### Конструкторы, создание объектов через "new"
Что такое конструкторы в js ? Что происходит, когда мы создаем объект через new ?


### Прототипы, наследование
Как работает прототипное наследование в js ?


### Классы
Что такое классы в js ? Чем они отличаются от функций ? Это что-то принципиально новое ? Как классы работают с наследованием ? Что делает extends



### Функции
Как задать дефолтное значение аргументу функции ?

Function Expression в сравнении с Function Declaration

### Общие
Где обучаешься? Из каких источников берешь информацию, что читаешь, сколько времени уделяешь своему обучению?

Почему ты хочешь к нам на стажировку? Какова твоя мотивация?

Почему хочешь на стажировку? Почему именно МТС? Чего ожидаешь от стажировки?

Расскажите о вашем опыте разработки. расскажите о своих должностных обязанностях. Доводилось ли вам работать в команде? В каких ОС вы работали?


### Общие технические
Работал ли ты с фреймворками? Что больше нравится React или Vue?

Работал ли с Node.js? Настраивал backend?

Ты работаешь в офисе в Москве и сделал красную кнопку, а тестировщик, который работает на удаленке из Владивостока, получил на тестирование твой год, посмотрел и говорит, что кнопка синяя. Предположи, почему так и что ты будешь делать в такой ситуации ?

### методологии разработки
Какие методы управления проектами используете? Как получаешь задачи, от кого? Знаешь о Scrum?




# React
Расскажи про жизненный цикл компонента в React

В чем отличие функциональных компонентов от классовых?

Назови методы жизненного цикла классового компонента ? Чем отличаются классовые компоненты от функциональных ? Расскажи, что делают хуки useState и useEffect ? Что передается вторым аргументом в useEffect ? Что передается в useState ?


# HTML/CSS
Чем отличаются блочные, инлайновые и инлайново-блочные элементы?

Расскажи про flexbox. Где уместно использовать? Какие параметры имеют флексы?

Расскажи про grid. Где уместно использовать? Какие параметры имеют гриды?

Чем абсолютное позиционирование отличается от фиксированного?

Что такое БЭМ? Чем элементы отличаются от блоков? В чем суть БЭМ’а?

Работал ли ты с препроцессорами? Зачем они нужны?

На чем ты обычно делаешь сетку сайта ? Что знаешь о флексах ? Как выровнять элемент по центру с помощью flex ? Как изменить позиционирование элементов, чтобы они отобразились по вертикали ?

Рендеринг страницы: что такое reflow и repaint



# Задачи

### на замыкание
```javascript
var i = 0

function printI() {
  setTimeout(() => console.log(i), 10)
}

for (i = 0; i < 10; i++) printI()
```
Почему выводится 10 раз 10? Как сделать так, чтобы выводилось от 1 до 10?

---
Напиши фабрику счетчиков, используя замыкания

---

### на делегирование событий
Есть огромная таблица (500 на 500) с ячейками, у каждой ячейки есть “условный” button, при нажатии на который происходит event, как бы ты это реализовал?

### на асинхронное программирование, промисы, promise, async/await
---
```javascript
Promise.resolve('a')
  .then(x => x + 'b')
  .catch(x => x + 'c')
  .catch(x => x + 'd')
  .then(x => x + 'e')
  .then(console.log)
```
Что будет в консоли ? а если поменять resolve на reject ?

---

```javascript
setTimeout(() => console.log('1'))

Promise.resolve().then(() => console.log('2'))

console.log('3')
```
Что будет в консоли?

---

### на конструкторы
Напиши конструктор Person, чтобы при вызове fullName в консоли было ‘Alex Petrov’
```javascript
const person = new Person('Alex', 'Petrov')
const name = person.fullName()
```


### на алгоритмы и структуры данных
---
Отсортируй массив [0, 1, 0, 1, 0, 0, 1, 1, 0] так, чтобы слева были нули, а справа единицы, не используя метод sort и сделав сортировку максимально быстрой

---

представим, что есть 3 кассы (cash) и очередь из клиентов (customers), каждый клиент занимает определенное время расплачиваясь в кассе, нужно определить сколько времени займет обслуживание всех клиентов
клиент из очереди может пройти к кассам только в том случае, если какая-то из них свободна

например:
в cash мы передаем кол-во касс, а в customers массив, состоящий из времени, которое требуется на обслуживание каждого клиента в том порядке, в котором была очередь клиентов

```javascript
function maxTime(customers, cash) {
  // ...код
}

maxTime([3, 20, 4, 1, 5, 6], 3) // вернет результат 20
```

---

Написать функцию, которая принимает две строки и смотрит, совпадают ли все символы первой строки с символами второй строки (важно учесть последовательность)

```javascript
# fuzzysearch('car', 'cartwheel')		// true
# fuzzysearch('cwhl', 'cartwheel')		// true
# fuzzysearch('cwheel', 'cartwheel')		// true
# fuzzysearch('cartwheel', 'cartwheel')	// true
# fuzzysearch('cwheeel', 'cartwheel')		// false
# fuzzysearch('lw', 'cartwheel')		// false
```
---

### верстка/html/css
На сайте нужно nav-menu с ссылками на другие страницы. Расскажи как бы ты его реализовал?

---
Что будет, если <span> задать position: absolute; ?
```
  <div class="container">
    Lorem ipsum <span class="incorporate">dolor sit amet</span>, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
  </div>
  
  <!--
    .incorporate {
      position: absolute;
    }
  -->
```
---

Назови сколько сможешь способов выровнять элемент по центру по вертикали, горизонтали и по двум осям сразу

---
