# **Мастерская. Анализ данных вакансий Data Analyst и Data Science**
**Цель исследования**

Выявить различия в предлагаемых вакансиях для Аналитиков данных и специалистов по Data Science.e

**Используемые библиотеки**

    - pandas
    - numpy
    - matplotlib
    - seaborn
    - plotly

**Исходные данные**

Данные получены из API HH.ru. Данные прошли предобработку и очистку.

**Шаги исследования**

1. Предобработка данных.

2. Исследовательский анализ данных.

3. Выявление грейда требуемых специалистов по названию вакансии или по колонке с требуемым опытом.
4. Определение доли грейдов Junior, Junior+, Middle, Senior среди вакансий Аналитик данных и Специалист по Data Science.
5. Определение типичного места работы для Аналитика данных и специалиста по Data Science по следующим параметрам:

    - ТОП-работодателей
    - зарплата
    - тип занятости
    - график работы
    - отдельно для грейдов Junior, Junior+, Middle, Senior.

6. Определение, какие навыки спрашивают чаще - твердые или мягкие. К какому грейдуи к какой специальности требований больше.

7. Определение наиболее желаемых кандидатов на вакансии Аналитик данных и Специалист по Data Science по следующим параметрам:

    - самые важные hard-skils
    - самые важные soft-skils
      
отдельно для грейдов Junior, Junior+, Middle, Senior.

8. Расчет помесячной динамику количества вакансий для Аналитика данных и специалиста по Data Science. 
Отдельно для грейдов Junior, Junior+, Middle, Senior.

9. Формулирование выводовы и рекомендаций.

Исходные данные:
  - Анализ проводится на основе данных полученных из API сайта HH.ru. Данные прошли предобработку и очистку.

Ссылки на данные:

    - vacancies_ds.xlsx - вакансии специалиста по Data Science. ссылка для скачивания: https://disk.yandex.ru/d/en_e87RKy9akHg
    
    - vacancies_da.xlsx - вакансии Аналитика данных. ссылка для скачивания: https://disk.yandex.ru/d/en_e87RKy9akHg

Описание полей в данных:

    - id: Уникальный идентификатор вакансии
    - name: Название вакансии
    - published_at: Дата публикации
    - alternate_url- Ссылка на вакансию
    - type- Статус вакансии на момент получения данных от api и передачи их в базу
    - employer- Работодатель
    - department- Работодатель, отдел
    - area - Регион места работы
    - experience - Требуемый опыт работы
    - key_skills - Ключевые навыки, в том числе найденные при анализе полного текста вакансии. Поле генерируется после - получения информации от api
    - schedule - График работы
    - employment - Тип занятости
    - description - Описание вакансии
    - description_lemmatized - Лемматизированное описание вакансии
    - salary_from - Нижняя граница предлагаемой заработной платы
    - salary_to - Верхняя граница предлагаемой заработной платы
    - salary_bin - Категория зарплаты
    - key_skills_from_key_skills_field - Ключевые навыки из поля вакансии key_skills
    - hard_skills_from_description - “Твердые” навыки, найденные при обработке полей с навыками. Поле генерируется после получения информации от api
    - soft_skills_from_description - “Мягкие” навыки, найденные при обработке полей с навыками. Поле генерируется после получения информации от api.
