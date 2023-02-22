# yandex_practicum
# Проекты из учебы в ЯндексПракикуме:
## Проект по SQL
### Данные
#### Таблица books:

- идентификатор книги;
- идентификатор автора;
- название книги;
- количество страниц;
- дата публикации книги;
- идентификатор издателя.

#### Таблица authors:

- идентификатор автора;
- имя автора.

#### Таблица publishers

- идентификатор издательства;
- название издательства;

#### Таблица ratings

- идентификатор оценки;
- идентификатор книги;
- имя пользователя, оставившего оценку;
- оценка книги.

#### Таблица reviews

- идентификатор обзора;
- идентификатор книги;
- имя пользователя, написавшего обзор;
- текст обзора.

### Задача.
Моя первая задача как аналитика — проанализировать базу данных. В ней — информация о книгах, издательствах, авторах, а также пользовательские обзоры книг. Эти данные помогут сформулировать ценностное предложение для нового продукта. Нужно выполнить 5 задачи:

- Посчитать, сколько книг вышло после 1 января 2000 года;
- Для каждой книги посчитать количество обзоров и среднюю оценку;
- Определить издательство, которое выпустило наибольшее число книг толще 50 страниц — так мы исключим из анализа брошюры;
- Определить автора с самой высокой средней оценкой книг — учитывайте только книги с 50 и более оценками;
- Посчитайть среднее количество обзоров от пользователей, которые поставили больше 50 оценок.

## Project-Telecom
### Данные:
В работу поступило два датасета, которые характеризуют использование услуг «НуПозвони»:
dataset:
- идентификатор клиента,
- дата статистики;
- направление вызовов: out — исходящий вызов, in — входящий;
- маркер внутренних и внешних вызовов (вызовы между сотрудниками одного колл-центра называют внутренними, остальные — внешними);
- идентификатор оператора;
- маркер пропущенных вызовов;
- количество звонков;
- длительность всех звонков без учёта времени ожидания;
- длительность всех звонков с учётом времени ожидания.
clients:
- идентификатор клиента;
- тарифный план клиента;
- дата регистрации клиента в сервисе.

### Задача.
Для предотвращения оттока клиентов, нужно провести ежеквартальный мониторинг активных клиентов, которые экономически неэффективно используют услуги на своих тарифах и могут снизить свои расходы, если перейдут на более выгодными для них тарифы, и оценить изменения выручки компании. Такой мониторинг будем делать систематически, раз в три месяца. Для достижения цели нужно определить активных клиентов, найти клиентов, которые неоптимально расходуют свои тарифы (сколько переплачивают), искать клиенту наиболее выгодные тарифы. Нам нужно также предложить возможные пути по минимизации потерь компании, если будет осуществлен перевод всех активных клиентов на более выгодные для них тарифы.

## Проект по А/В тесту.
### Данные:
Нам даны 4 данных

1. Календарь маркетинговых событий на 2020 год:
- название маркетингового события;
- регионы, в которых будет проводиться рекламная кампания;
- дата начала кампании;
- дата завершения кампании.
2. Пользователи, зарегистрировавшиеся с 7 по 21 декабря 2020 года:
- идентификатор пользователя;
- дата регистрации;
- регион пользователя;
- устройство, с которого происходила регистрация.
3. Действия новых пользователей в период с 7 декабря 2020 по 4 января 2021 года:
- идентификатор пользователя;
- дата и время покупки;
- тип события;
- дополнительные данные о событии. Например, для покупок, purchase, в этом поле хранится стоимость покупки в долларах.
4. Таблица участников тестов:
- идентификатор пользователя;
- название теста;
- группа пользователя.

### Задача.
#### Провести оценку результатов A/B-теста. В нашем распоряжении есть датасет с действиями пользователей, техническое задание и несколько вспомогательных датасетов.
- Оценить корректность проведения теста
- Проанализировать результаты теста.
#### Чтобы оценить корректность проведения теста, проверить:
- пересечение тестовой аудитории с конкурирующим тестом,
- совпадение теста и маркетинговых событий, другие проблемы временных границ теста.

## Используемые библиотеки
- pandas
- numpy
- scipy
- matplotlib
- plotly
- seaborn
- math
- sqlalchemy
