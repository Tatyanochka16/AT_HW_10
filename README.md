# Тест-план

Задание: тестирование возможности записаться на обучение профессии «Инженер по тестированию».

## 1. Сценарий перехода к форме записи на курс "Инженер по тестированию"

1. Переход через вкладку "Каталог курсов" в заголовке сайта:
   * Открыть страницу сайта http://netology.ru/ ;
   * Выбрать вкладку "Каталог курсов";
   * В открывшемся каталоге выбрать кнопку "Программирование";
   * В открывшемся каталоге выбрать курс "Инженер по тетсированию";
   * В открывшейся странице заполнить форму  и нажать кнопку "Записаться".
  
2. Переход через строку поиска: 
   * Открыть страницу сайта http://netology.ru/ ;
   * Выбрать вкладку "Каталог курсов"; 
   * Ввести в строке поиска "Инженер по тестированию";
   * В открывшехся результатах поиска выбрать курс "Инженер по тетсированию";
   * В открывшейся странице заполнить форму  и нажать кнопку "Записаться".

3. Переход через раздел "Направления обучения":
   * Открыть страницу сайта http://netology.ru/ ;
   * Прокрутить страницу до раздела "Направления обучения";
   * Выбрать раздел "Программирование";
   * В открывшемся каталоге выбрать курс "Инженер по тетсированию";
   * В открывшейся странице заполнить форму  и нажать кнопку "Записаться".

4. Переход через раздел "Направления обучения" и кнопку "Полный каталог":
   * Открыть страницу сайта http://netology.ru/ ;
   * Прокрутить страницу до раздела "Направления обучения";
   * Нажать на кнопку "Полный каталог";
   * В открывшемся каталоге выбрать курс "Инженер по тетсированию";
   * В открывшейся странице заполнить форму  и нажать кнопку "Записаться".

5. Переход через раздел "Направления обучения" и поисковую строку:
   * Открыть страницу сайта http://netology.ru/ ;
   * Прокрутить страницу до раздела "Направления обучения";
   * Нажать на кнопку "Полный каталог";
   * Ввести в строке поиска "Инженер по тестированию";
   * В открывшехся результатах поиска выбрать курс "Инженер по тетсированию";
   * В открывшейся странице заполнить форму  и нажать кнопку "Записаться".
  
## 2. Сценарии автоматизированного тестирования заполения формы

|Сценарий|Вводимые данными|Ожидаемый результат|
|---|---|
|Позитивные сценарии:|
|Отправка формы, заполненной валидными данными|Все поля заполнены валидными данными|Сообщние об успешной отправке формы|
|Негативные сценарии|
|Отправка формы с невалидными данными в поле "Имя" и валидным значением номера телефона|1. Ввод в поле "Имя" специальных символов, не подразумеваемых докментацией; 2. Ввод в поле "Имя" цифр; 3. Ввод в поле "Имя" имя, имеющего длину больше разрешенного документацией; 4. Ввод в поле "Имя" имя, имющего длину меньше разрешенного документацией; 5. Ввод в поле "Имя" иероглифоф| Сообщение об ошибке. Неверно заполнены необходимые поля|

|Отправка формы с валидными данными в поле "Имя" и невалидными данными номера телефона|1. Ввод в поле "Номер телефона" букв; Ввод в поле "Номер телефона" специальных символов, не подразумеваемых докментацией; 2. Ввод в поле "Номер телефона" номера длинней 11 цифр; 3. Ввод в поле "Номер телефона" номера короче 11 цифр; 4. Ввод в поле "Номер телефона" несуществующего номера; 5. Ввод в поле "Номер телефона" иероглифоф|| Сообщение об ошибке. Неверно заполнены необходимые поля|

|Отправка формы с валидными данными в поле "Имя" и пустым полем "Номер телефона"|Ввод валидных данных в поле "Имя", поле "Номер телефона" остается пустым| Сообщение об ошибке. Неверно заполнены необходимые поля|
|Отправка формы с валидными данными в поле "Номер телефона" и пустым полем "Имя"|Ввод валидных данных в поле "Номер телефона", поле "Имя" остается пустым| Сообщение об ошибке. Не заполнены необходимые поля|

|Отправка формы с валидными данными в поле "Имя" и пустым полем "Номер телефона"|Ввод валидных данных в поле "Имя", поле "Номер телефона" остается пустым| Сообщение об ошибке. Не заполнены необходимые поля|

|Отправка формы с пустым полем "Номер телефона" и пустым полем "Имя"|Поля "Номер телефона" и "Имя" остаютсяя пустыми|Сообщение об ошибке. Не заполнены необходимые поля|

## 3. Перечень используемых инструментов

1. InteleiJ IDEA -  среда разработки программного обеспечения для многих языков программирования, в частности Java. 
2. JDK - комплект разработчика приложений на языке Java, включающий в себя компилятор Java (javac), стандартные библиотеки классов Java, примеры, документацию, различные утилиты и исполнительную систему Java.
3. Gradle -  система автоматической сборки и разработки и развертывания Java.
4. JUnit — фреймворк для модульного тестирования программного обеспечения на языке Java.
5. Selenide - это автоматизированная система тестирования программного обеспечения, используемая для написания программных кодов, а так же для создание скриптов, с помощью которых становится проще тестировать работу веб-продуктов.
6. REST Assured — это библиотека Java для тестирования API RESTful, широко используется для тестирования веб-приложений на базе JSON и XML.  
7. Facker - библиотека для генерации случайных данных, для упрощения автоматизации тестирования.
8. Allure - инструмент для создания и просмотра графических отчётов. Для составления удобных и наглядных репортов по результатам тестирования. 
9. Git - это распределённая система контроля версий,  позволяет следить за происходящими изменениями, а также работать над одним заданием одновременно нескольким разработчикам.

## 4. Перечень необходимых разрешений, данных и доступов

1. Разрешение на тестирования у правообладателя сайта;
2. Доступ технической документации;
3. Доступ к API;
4. Доступ к базам даных.

## Перечень и описание возможных рисков при автоматизации

1. Возможное изменение кода, селекторов, структуры сайта. Тогда появится необходимость дорабатывать тесты под новые данные.
2. Эффект пестицида. Повторное применение тех же тестов и тех же методик приводит к тому, что в продукте остаются дефекты, о которых не подумали или не узнали. 
3. Остается необходимость в ручном тестировании, так как некоторые тесты проще, быстрее и дешевле сделать руками.
4. Нет возможности UX-тестирования.
5. Остановка работы на территории РФ некоторых необходимых инструментов. В таком случае придется искать замену и перенастраивать тесты под аналоги.

## 5. Перечень необходимых специалистов для автоматизации

Для проведения автоматизации данной возможности понадобится один специалист по тестированию, с необходимыми навыками работы. 

## 6. Интервальная оценка с учётом рисков в часах

Для выполнения данного задания специалисту потребуется от нескольких часов до 2-3 недель. Все зависит от уровня подготовки специалиста, имеющихся уже интсрументов и документации. 
Если у специалиста уже имеется все необходимое (все документы на руках, установлны все инструменты и поготовлены среды, а так же имеется опыт и накоплены практики тестирования), то на данную задачу понадобится 48 часов.
Если для тестирования необходимо еще запрашивать документацию и подготавливать среду, в которой специалисту еще нужно разобраться, то процесс может затянуться на недели.


