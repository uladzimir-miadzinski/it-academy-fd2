## Функции. Продвинутая работа

Задания выполняется в папке репозитория `/js/functions/pro`.  
Для каждого задания создается файл с номером задания по списку, к примеру `/js/functions/pro/task-1.js`  
В коде каждого файла с решением в самом верху в комментарии добавьте текст решаемого задания.  
В ответ на задание прикрепить ссылку на Pull-Request

### Теория:
* https://learn.javascript.ru/recursion 
* https://habr.com/ru/post/337030/
* https://learn.javascript.ru/rest-parameters-spread-operator
* https://learn.javascript.ru/closure
* https://developer.mozilla.org/ru/docs/Web/JavaScript/Closures
* https://learn.javascript.ru/function-object
* https://youtu.be/rh1mP02NFoM (очень крутое объяснение которое я добросовестно заимствовал, сам когда-то понял только на этом примере)
* https://youtu.be/Pc6qX0HfDs4 (старайтесь создавать больше чистых функций и будет вам счастье во всём)
* https://developer.mozilla.org/en-US/docs/Web/API/console
* https://learn.javascript.ru/call-apply-decorators
* https://learn.javascript.ru/bind
* https://learn.javascript.ru/arrow-functions
* https://learn.javascript.ru/object-methods

### Задания:
1. https://learn.javascript.ru/task/sum-many-brackets (частая задача на собеседованиях, попробовать решить, если не сможете в течении часа, посмотреть 
и разобрать решение, в случае если не поймёте самостоятельно, выделим время на лекции для разбора)
1. *Function as an Object*.  
Создайте функцию `str()`, которая принимает один строчный параметр и выводит в консоль `'String is non empty'`, если параметр - непустая строка и `'String is empty'`, если параметр – пустая строка.  
Создайте функцию `str.isNonEmptyStr()`, как свойство функции `str`.  
Эта функция должна принимать один параметр и возвращать `true`, если параметр непустая строка, иначе `false`.  
Используйте эту функцию для реализации условия в основной функции.  
Тестовые данные:
     ```
     str.isNonEmptyStr(), result = false
     str.isNonEmptyStr(''), result = false
     str.isNonEmptyStr('a'), result = true
     str.isNonEmptyStr(1), result = false
     str(), console.log('String is empty')
     str('a'), console.log('String is non empty')
    ```
1. Создайте функции `toConsoleLog`, `toConsoleError`, `toConsoleTrace`, `toConsoleTable` с одним параметром.  
Функции должна выводить значение параметра в консоль в соответствующем режиме.  
Создайте функцию `splitToWords` с двумя параметрами: `msg` и `callback`.  
Функция должна разделять строку на слова и использовать колбек для отображения слов.  
Если второй параметр не задан, функция должна возвращать массив слов.
1. *Function as a Result*.  
Создайте функцию `copyright` с одним параметром - значок копирайта, которая должна возвращать другую функцию с одним параметром.  
Возращаемая функция должна прибавлять знак © ('\u00A9') (*в случае если он был передан в `copyright` функцию или как значение по умолчанию внутри функции, если параметр не был передан*) вначале своего параметра и возвращать результат. 
Тестовые данные:
    ```
    console.log( copyright('\u00A1')('EPAM') ); result = ¡ EPAM.
    console.log( copyright('\u00A9')('EPAM') ); result = © EPAM.
    console.log( copyright()('EPAM') ); result = © EPAM.
    ```
1. *Arguments Object, Rest*.  
Создайте функцию `parts`, которая принимает неизвестное количество параметров. Каждый параметр – это группа предложений.  
Функция должна вырезать из параметра подстроку, начиная с символа двоеточие `:` и заканчивая символом точка `.`.  
Функция должна возвращать массив подстрок. Используйте *Function Definition Expression (FDE)*.
Тестовые данные:
    ```
    param1 = "This is the first sentence. This is a sentence with a list of items: cherries, oranges, apples, bananas."
    param2 = "This is the second sentence. This is a sentence with a list of items: red, blue, yellow, black."
    result = ["cherries, oranges, apples, bananas", "red, blue, yellow, black"].
    ```
1. Создайте литерал объекта employee со следующими свойствами: `name: 'Ann'`, `work` – функция, которая выводит в консоль сообщение `"I am Ann. I am working..."`. Имя `Ann` должно быть взято из свойства `name`
Тестовые данные:  
    ```
    employee.work()  результат в консоле "I am Ann. I am working..."
    ```
1. *Borrow Method - call/apply/bind*. Создайте литерал объекта person со свойством `name`. Вызовите метод `work` объекта employee из предыдущего задания.
1. *Memoization*. Создать функцию `fiboMemo` для вычисления чисел Фибоначчи по формуле `F0 = 0, F1 = 1, Fn = Fn-1 + Fn-2`.  
Функция должна хранить те значения, которые она уже вычисляла.  
Используя методы `console.time()`, `console.timeEnd()` определите время вычисления функции `fibo` и функции `fiboMemo`.
