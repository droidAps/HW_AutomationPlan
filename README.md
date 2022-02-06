# План автоматизации тестирования возможности записи на курс "Тестировщик ПО"

## Содержание:
1. Перечень автоматизируемых сценариев
2. Перечень используемых инструментов
3. Перечень необходимых разрешений/данных/доступов
4. Перечень и описание возможных рисков при автоматизации
5. Перечень необходимых специалистов для автоматизации
6. Интервальная оценка с учётом рисков

## Перечень автоматизируемых сценариев
### Сценарии перехода на страницу курса "Тестировщик ПО":
#### 1. Сценарий перехода через "Каталог курсов".
Шаги воспроизведения:
1. Открыть [главную страницу](https://netology.ru) веб-сайта Нетологии;
2. Нажать на элемент "Каталог курсов" ([Каталог курсов](img.png));
3. Навести курсор на направление "Программирование" ([Программирование](img_1.png));
4. Выбрать курс "Тестировщик ПО" из списка "Для начинающих" ([Тестировщик ПО](img_2.png)).

Ожидаемый результат:
открытие [страницы курса "Тестировщик ПО"](https://netology.ru/programs/qa).

#### 2. Сценарий перехода через уровень "НЕО".
Шаги воспроизведения:
1. Открыть [главную страницу](https://netology.ru) веб-сайта Нетологии;
2. Выбрать уровень "НЕО" ([уровень "НЕО"](img_3.png));
3. Пролистать страницу до списка курсов и нажать на чекбокс "Программирование" ([чекбокс "Программирование"](img_5.png));
4. Выбрать курс "Тестировщик ПО" из списка ([Тестировщик ПО](img_6.png)).

Ожидаемый результат:
открытие [страницы курса "Тестировщик ПО"](https://netology.ru/programs/qa).

#### 3. Сценарий перехода через "Полный каталог".
Шаги воспроизведения:
1. Открыть [главную страницу](https://netology.ru) веб-сайта Нетологии;
2. Нажать на элемент "Каталог курсов" ([Каталог курсов](img.png));
3. Нажать на элемент "Полный каталог" ([Полный катало](img_7.png));
4. Ввести в поле поиска запрос "Тестировщик ПО" ([Поле поиска](img_8.png));
5. Выбрать курс "Тестировщик ПО" ([Тестировщик ПО](img_9.png)).

Ожидаемый результат:
открытие [страницы курса "Тестировщик ПО"](https://netology.ru/programs/qa).

### Сценарии записи на обучение профессии "Тестировщик ПО":
#### 1. Сценарий записи на курс через кнопку "Записаться" в верхней части страницы.
Шаги воспроизведения:
1. Открыть [страницу курса "Тестировщик ПО"](https://netology.ru/programs/qa);
2. Нажать на кнопку "Записаться" в верхней части страницы ([Кнопка "Записаться"](img_10.png));
3. Сгенерировать тестовые данные (русское имя и номер телефона) с помощью библиотеки Faker;
4. Ввести в соответствующие поля тестовые данные ([Соответствующие поля](img_12.png));
5. Нажать на кнопку "Записаться" внутри формы ([Кнопка "Записаться" внутри формы](img_13.png));
6. Сравнить данные, записанные в базу данных, с тестовыми.

Ожидаемый результат:
- Появление сообщения об успешной записи (шаг воспроизведения №5);
- Соотвествие данных, записанных в базу данных, тестовым (шаг воспроизведения №6).

#### 2. Сценарий записи на курс через кнопку "Записаться" в поле "Гарантия возврата денег".
Шаги воспроизведения:
1. Открыть [страницу курса "Тестировщик ПО"](https://netology.ru/programs/qa);
2. Нажать на кнопку "Записаться" в поле "Гарантия возврата денег" ([Кнопка "Записаться"](img_14.png));
3. Сгенерировать тестовые данные (русское имя и номер телефона) с помощью библиотеки Faker;
4. Ввести в соответствующие поля тестовые данные ([Соответствующие поля](img_15.png));
5. Нажать на кнопку "Записаться на курс" внутри формы ([Кнопка "Записаться на курс"](img_16.png));
6. Сравнить данные, записанные в базу данных, с тестовыми.

Ожидаемый результат:
- Появление сообщения об успешной записи (шаг воспроизведения №5);
- Соотвествие данных, записанных в базу данных, тестовым (шаг воспроизведения №6).

#### 3. Сценарий записи на курс через форму записи в нижней части страницы.
Шаги воспроизведения:
1. Открыть [страницу курса "Тестировщик ПО"](https://netology.ru/programs/qa);
2. Сгенерировать тестовые данные (русское имя и номер телефона) с помощью библиотеки Faker;
3. Ввести в соответствующие поля формы записи в нижней части страницы тестовые данные ([Соответствующие поля](img_12.png));
4. Нажать на кнопку "Записаться" внутри формы ([Кнопка "Записаться" внутри формы](img_13.png));
5. Сравнить данные, записанные в базу данных, с тестовыми.

Ожидаемый результат:
- Появление сообщения об успешной записи (шаг воспроизведения №4);
- Соотвествие данных, записанных в базу данных, тестовым (шаг воспроизведения №5).

## Перечень используемых инструментов
#### 1. Junit5 - среда для создания и запуск тестов;
#### 2. Faker - библиотека для создания тестовых данных;
#### 3. Selenide - фреймворк для работы с веб-элементами.
#### 4. Apache Commons DbUtils — набор классов, делающих работу с JDBC проще.
#### 5. Драйвер, позволяющий подключаться к БД.

## Перечень необходимых разрешений/данных/доступов
#### 1. Разрешение на тестирование от руководства ООО "Нетология";
#### 2. Доступ к базе данных, содержащей данные о записи абитуриентов на курс.

## Перечень и описание возможных рисков при автоматизации
#### 1. При тестировании с использованием рабочих серверов появляется дополнительная нагрузка на них;
#### 2. Сложность в организации доступа к БД тестировщикам;
#### 3. Реализация и поддержка автотестов требует привлечения сотрудников (увеличение нагрузки на сотрудников).

## Перечень необходимых специалистов для автоматизации
#### 1. Тестировщик ПО с навыком автоматизации.

## Интервальная оценка с учётом рисков (в часах)
### 4-6 часов.
