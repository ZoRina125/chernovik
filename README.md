# Лабораторная работа №1. Введение в JavaScript

## Цель работы:
Познакомиться с основами JavaScript, научиться писать и выполнять код в браузере и в локальной среде, разобраться с базовыми конструкциями языка.

# Условие:
## Задание 1. Выполнение кода в браузере
1.Подготовка среды:

- Был установлен текстовый редактор  VS Code.
- Был установлен Node.js с официального сайта.
- Открываем DevTools в браузере, нажав F12 и выбрав вкладку Консоль.

2.Выполнение кода JavaScript в браузере

- Открыли консоль разработчика (F12 → Console).
- Написали команду console.log("Hello, world!"); и нажали Enter.

<img width="1116" height="230" alt="Screenshot 2026-02-10 221234" src="https://github.com/user-attachments/assets/413bc40a-dfe3-4695-bb02-b56ce1f290f9" />

- Записали в консоль 2 + 3 и получили такой результат:

<img width="530" height="130" alt="Screenshot 2026-02-11 172642" src="https://github.com/user-attachments/assets/1dc0099f-4754-47ff-a953-f051d6e9e7d5" />

3. Создание первой HTML-страницы с JavaScript
- Создаем файл index.html и вставляем в него следующий код:
     ```
  <!DOCTYPE html>
  <html lang="en">
  <head>
   <title>Привет, мир!</title>
  </head>
  <body>
    <script>
     alert("Привет, мир!");
     console.log("Hello, console!");
   </script>
  </body>
  </html>  
   ```
Откываем index.html в браузере и наблюдаем , как выполняется код:
<img width="1044" height="404" alt="Screenshot 2026-02-10 221437" src="https://github.com/user-attachments/assets/8766959d-cb86-43ab-b29f-186d690464c7" />


4.Подключение внешнего JavaScript-файла
Создаем файл script.js и добавляем в него код:
```
alert("Этот код выполнен из внешнего файла!");
console.log("Сообщение в консоли");
```
Подключаем файл в index.html, добавив в <head>
```
<script src="script.js"></script>
```
Открываем страницу в браузере:
<img width="1111" height="448" alt="Screenshot 2026-02-10 221832" src="https://github.com/user-attachments/assets/81319bcc-273d-4a78-9b71-7ea306d946a6" />


## Задание 2. Работа с типами данных
1. Объявление переменных и работа с типами данных.
В файле script.js создаем несколько переменных:
```
name - строка с  именем.
birthYear - число, представляющее год рождения.
isStudent - логическая переменная, указывающая, являюсь ли студентом
Вывели их в консоль
```
<img width="1189" height="840" alt="Screenshot 2026-02-10 223646" src="https://github.com/user-attachments/assets/14db7f8e-717b-45bf-9fc9-9a569b7ac9ca" />
 

2. Управление потоком выполнения (условия и циклы)
Добавили следующий код в script.js:
```
let score = prompt("Введите ваш балл:");
if (score >= 90) {
 console.log("Отлично!");
} else if (score >= 70) {
 console.log("Хорошо");
} else {
 console.log("Можно лучше!");
}

for (let i = 1; i <= 5; i++) {
 console.log(`Итерация: ${i}`);
}
```
<img width="566" height="254" alt="image" src="https://github.com/user-attachments/assets/1dbcaca8-29dc-4529-8e71-52d2f3beffb2" />

<img width="1276" height="822" alt="Screenshot 2026-02-10 223741" src="https://github.com/user-attachments/assets/ed1f9963-4e54-4280-9449-6283968390d9" />

Открываем страницу в браузере и наблюдаем, как работают условия и циклы.

[index.html](https://github.com/user-attachments/files/25239374/index.html)

 [script.js](https://github.com/user-attachments/files/25239357/script.js)
# Контрольные вопросы
## 1.Чем отличается var от let и const?

   var- это старый способ объявлять переменные в JavaScript. Такие переменные видны во всей функции, даже если объявлены внутри блока.
 let и const более новые и безопасные варианты, они работают только внутри фигурных скобок. let можно изменять, а const — нет. Поэтому чаще всего используют let и const.
 
## 2. Что такое неявное преобразование типов?

Это когда JavaScript сам меняет тип данных, чтобы выполнить действие. Это происходит автоматически, без указаний программиста

## 3.Как работает == и === ?
== сравнивает значения и может менять типы данных. === сравнивает и значение, и тип, ничего не меняя. Например 5 == "5" даст true , а  5 === "5" даст false. В коде чаще используют ===, потому что это безопаснее.
# Источники:
- Материалы лабораторной №1 на сайт курса (https://moodle.usm.md) 
