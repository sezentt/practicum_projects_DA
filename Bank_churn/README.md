# Описание проекта - Анализ оттока клиентов банка
<b>Цель проекта</b>: Проанализировать отток клиентов банка «Метанпром» и выявить клиентские сегменты, склонные к уходу, с применением методов кластеризации. Результаты анализа могут быть использованы для разработки стратегий удержания клиентов.

## Данные
Датасет содержит данные о клиентах банка «Метанпром». Банк располагается в
Ярославле и областных городах: Ростов Великий и Рыбинск.

Описание столбцов:
- `USERID` — идентификатор пользователя,
- `score` — баллы кредитного скоринга,
- `city` — город,
- `gender` — пол,
- `age` — возраст,
- `equity` — количество баллов собственности
- `balance` — баланс на счёте,
- `products` — количество продуктов, которыми пользуется клиент,
- `credit_card` — есть ли кредитная карта,
- `last_activity` — активный клиент,
- `EST_SALARY` — оценочный доход клиента,
- `сhurn` — признак оттока.

## Задачи
<b>Задачи проекта</b>:
1. Загрузка и изучение данных:
    - Загрузить данные, положить их в датафрейм.
    - Изучить общую информацию, описать. 
2. Предобработка данных:
    - Работа со столбцами (при необходимости).
    - Анализ наличия и природы пропущенных значений.
    - Обработка пропусков (удаление, заполнение или иные стратегии).
    - Кодирование категориальных признаков для дальнейшего анализа.
    - Поиск и устранение дублей (если имеются).
    - Оценка распределения значений в столбцах, выявление выбросов.
3. EDA (исследовательский анализ данных):
    - Анализ распределения признаков в разрезе оттока.
    - Выявление взаимосвязей между churn и другими признаками (корреляционный анализ).
    - Построение портретов клиентов, склонных к оттоку.
4. Статистический анализ:
    - Проверка статистических гипотез о различиях между ушедшими и оставшимися клиентами.
    - Обоснование выбора статистических тестов.
    - Анализ значимости факторов.
5. Кластеризация клиентов:
    - Формулировка задачи машинного обучения: Задача кластеризации - выделение сегментов (кластеров) клиентов на основе схожих характеристик.
    - Выбор метода кластеризации: K-Means (если данные чётко разделяются, возможна корректировка метода после EDA).
    - Выбор метрики для кластеризации: евклидово расстояние (для K-Means).
    - Оценка оптимального числа кластеров (метод Elbow).
    - Подготовка данных: масштабирование признаков, отбор релевантных характеристик.
    - Анализ полученных кластеров: интерпретация характеристик клиентов в каждом сегменте.
6. Приоритизация сегментов:
    - Определение сегментов с наибольшей склонностью к оттоку.
    - Выделение ключевых характеристик рисковых клиентов.
7. Формирование рекомендаций:
    - Разработка стратегии взаимодействия с каждым выделенным сегментом.
    - Определение потенциальных мер по снижению оттока.
    - Выявление возможностей персонализированных предложений клиентам.

## Используемые библиотеки
*pandas*<br>
*numpy*<br>
*matplotlib*<br>
*seaborn*<br>
*scipy*<br>
*sklearn*<br>
