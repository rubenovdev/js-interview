
# Задачи

### интересные задачи

```javascript
var foo = {n: 1};
var bar = foo;
foo.x = foo = {n: 2};

console.log(foo.x);
```

### На типы данных, преобразования
```javascript
  console.log(typeof (1 / []))
```

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

что будет в консоли
```javasript
for (var i = 0; i < 10; i++) {
  (i => {
    setTimeout(() => {
      console.log(i);
    }, 1000);
  })(i);
}
```

---
Напиши фабрику счетчиков, используя замыкания

---

### на делегирование событий
Есть огромная таблица (500 на 500) с ячейками, у каждой ячейки есть “условный” button, при нажатии на который происходит event, как бы ты это реализовал?

---

Есть список (ul),  в нем 10000 строк (li), как сделать так, чтобы при клике на любой li выводилось его содержимое с максимальной экономией памяти?

---

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

```javascript
// /* Promise.resolve(1)
// .then( Promise.resolve(2), (res) => res + 3)
// .catch( res => res + 4)
// .then( res => console.log(res), res => console.log(res + 5)); */
```

---

### на конструкторы
Напиши конструктор Person, чтобы при вызове fullName в консоли было ‘Alex Petrov’
```javascript
const person = new Person('Alex', 'Petrov')
const name = person.fullName()
```

### на классы
Перепиши классы с наследованием в код на ES5

### на хостинг переменных
Что выводится в консоль?
```javascript
var a = 2;
function {
    a+=1
    console.log(a);
    var a = 1;
}
```
Почему выводится undefined?

---

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

Как поменять два слова в строке местами? Например, есть ‘Hello world’ и как сделать ‘world Hello’? (подсказка: это делается двумя методами)

---

На листе бумаги написать функцию, которая получает число и, если число делится на 3, тогда выводится “Hello”, если делится на 5, тогда “world”, если делится на 15, тогда “Hello world”

---

Перед тобой стоит задача: написать функция , которая принимает на вход слово и возвращает его склонения, как ты ее реализуешь ?

---

Найди абсолютную разницу между элементами массива

---

```javascript
Написать функцию sum, которая работает таким образом: sum(a)(b)(n) = a+b+n

Решение
Для двух значений

const sum = a => b => a + b

--

Для нескольких sum()()()()()()
function sum(a) {
  let currentSum = a

  function f(b) {
    currentSum += b
    return f
  }

  f.toString = () => currentSum

  return f
}


```

---

Глубокое клонирование объектов/массивов. Как его сделать

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
