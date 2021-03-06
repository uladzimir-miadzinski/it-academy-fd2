## Git. NodeJS. Настройка окружения.

Задания выполняются на github.com в *публичном репозитории*.  
Для всех тренировочных заданий по JavaScript у нас будет папка `/js` в корне репозитория.  

### Теория:
* https://habr.com/ru/company/mailru/blog/493816/ (о git в одной статье)
* https://youtu.be/PEKN8NtBDQ0 (видеоруководство о git кто пропустил fd1 или кто забыл)

### Задания:
1. Создать аккаунт на https://github.com (рекомендую имя-фамилия на латинице как в паспорте, например uladzimir-miadzinski т.к. ваш репозиторий потом вы будете скорее всего скидывать потенциальным работодателям и будет совсем неловко иметь логин super-telka или stalnye-iichki)
1. Создать git-репозиторий с названием нашей группы (см. в Discord, маленькими буквами)
1. Зайти в *Settings -> Manage access ->* нажать кнопку *Invite a collaborator*
    * Ввести имя пользователя *uladzimir-miadzinski*
1. Зайти в *Settings -> Webhooks ->* нажать кнопку *Add webhook*
    * Заполнить *Payload URL* ссылкой, которая находится в закреплённом сообщении вашей группы в *Discord*.
    * Установить *Content type* - *application/json*
    * На этой же странице настроить какой информацией делится: установить radio-кнопку в *Let me select individual events*. и выбрать следующее:
        * *Pull request review comments*
        * *Pull request reviews*
        * *Pull requests*
    * На *Active* должна быть установлена галочка
1. При создании репозитория должна быть создана ветка *main* или *master*.
1. Зайти в *Settings -> Branches -> Branch protection rules* и нажать кнопку *Add rule*
    * Branch name pattern заполнить *main* или *master*
    * Установить галочку на *Require pull request reviews before merging*. 
    * Проверить что установлено: *Required approving reviews: 1*
1. Создать новую ветку от главной с любым именем, создать *README.MD* файл (или отредактировать существующий), добавив в него первой строкой Ваше ФИО и создать проверочный *Pull-Request* на объединение изменений с основной веткой
1. Если всё выполнено верно, то в группе в *Discord* сработает *Webhook* и бот автоматически напишет в *Discord* что вы создали *Pull-Request* который можно проверять
1. Установить NodeJS LTS http://nodejs.org/ (для Windows 7 использовать NodeJS 8)
1. В ответ на задание прикрепить ссылку на ваш репозиторий
