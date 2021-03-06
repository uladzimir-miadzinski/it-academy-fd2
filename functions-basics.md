## Функции

Задания выполняется в папке репозитория `/js/functions/basics`.  
Для каждого задания создается файл с номером задания по списку, к примеру `/js/functions/basics/task-1.js`  
В коде каждого файла с решением в самом верху в комментарии добавьте текст решаемого задания.  
В ответ на задание прикрепить ссылку на Pull-Request

### Теория:
* https://learn.javascript.ru/function-basics
* https://learn.javascript.ru/new-function (Function Constructor)
* https://learn.javascript.ru/function-expressions
* https://learn.javascript.ru/arrow-functions-basics
* https://learn.javascript.ru/closure#iife (пока что читаем только про IIFE, потом обязательно всеравно придётся читать это всё и даже учить наизусть)
* Тег-функции (0.5% шанс встретить в каком-либо коде, но узнать что такое есть полезно)   
https://codeburst.io/javascript-what-are-tag-functions-97682f29521b
* https://learn.javascript.ru/javascript-specials (подведение итогов по вводной части)
* https://learn.javascript.ru/introduction-browser-events
* http://jsraccoon.ru/es6-defaults (ES6 реализация - то, что нужно, но полезно знать все способы)

### Задания:
1. Создать функцию, которая выводит в консоль строчку в формате 'символ - код' для кодов в диапазоне 78000 - 78030 (все пары в диапазоне).  
Используйте `String.prototype.fromCodePoint()`.
1. Создайте тег-функцию `currency`, которая формитирует числа до двух знаков после запятой и добавляет знак доллара перед числом в шаблонном литерале.
1. Создайте функцию `conc`, которая должна конкатенировать значения двух параметров a и b и возвращать строку.  
Используйте *Function Declaration Statement (FDS)*. Вызовите функцию до ее объявления.  
Тестовые данные:  
    ```
    a = '1', b = '1', result = '11' 
    a = 1, b = 1, result = '11'
    ```
1. Создайте функцию comp, которая должна сравнивать значения двух параметров `a` и `b` и возвращать `1`, если они равны и `-1`, если они не равны.  
Используйте *Function Definition Expression (FDE)*. Вызовите функцию до ее объявления.  
Тестовые данные:
    ```
    a = 'abc', b = 'abc', result = 1
    a = 'abC', b = 'abc', result = -1
    ```
1. Создайте анонимную функцию, которая должна выводить сообщение `'message in console'` в коноль. Используйте ее как обработчик события *click* для кнопки.
1. Объявите две строчные переменные: params и body и проинициализируйте их строчными значениями, которые представляют список параметров и тело будущей функции.  
Создайте функцию, используя эту информацию с помощью *Function Constructor (FC)*. Вызовите эту функцию.
1. Объявите массив `arr = [1, 8, 3, 5, 12, 7, 9, 11]`. Используя стрелочные функции создайте новый массив из элементов `elem * elem`,  
которые меньше `100` и отсортируйте его по возрастанию. Выведите результат в консоль.
1. Создайте конструкцию, с помощью которой сразу выполниться выше реализованная функция `conc`. Используйте IIFE.
1. Создайте функцию `find(testString, test)`, которая должна возвращать позицию строки `test` в строке `testString`.   
Если второй параметр не задан, используйте `test = testString`. Используйте Function Definition Expression (FDE).
Тестовые данные:
    ```
    testString = 'abc', test ='b', result = 1
    testString = 'abc', result = 0
    testString = 'abc', test = 'd', result = -1
    testString = 'abc', test='a', test2='b', result = 0
    ```
1. Решать как для браузера. Создайте функцию-конструктор `Calculator`, который создаёт объекты с четырьмя методами:  
`read()` запрашивает два значения при помощи prompt и сохраняет их значение в свойствах объекта.  
`sum()` возвращает сумму введённых свойств.  
`multiply()` возвращает произведение введённых свойств.  
`history()` возвращает историю вызванных функций при работе с объектом начиная с момента его создания.
