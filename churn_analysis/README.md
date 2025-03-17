## [Анализ оттока водителей в компании такси](https://github.com/ElenaAnalyst/product_analytics/blob/main/churn_analysis/churn_analysis.ipynb)
Ознакомиться с файлом решения можно тут (нажать) ⤴️

### 🛠️ Стек:
<div>
<img src="https://img.shields.io/badge/python-white?logo=python&style=for-the-badge" title="Python" alt="Python" height=35"/>&nbsp;
<img src="https://img.shields.io/badge/pandas-white?logo=pandas&logoColor=blue&style=for-the-badge" title="Pandas" alt="Pandas" height="35"/>&nbsp;
<img src="https://img.shields.io/badge/numpy-white?logo=numpy&logoColor=blue&style=for-the-badge" title="Numpy" alt="Numpy" height="35"/>&nbsp;
<img src="https://img.shields.io/badge/-scipy.stats-FFF?style=for-the-badge&logo=scipy&logoColor=blue" title="scipy.stats" alt="scipy.stats" height="35"/>&nbsp;
<img src="https://img.shields.io/badge/-Seaborn-FFF?style=for-the-badge&logo=seaborn&logoColor=blue" title="Seaborn" alt="Seaborn" height="35"/>&nbsp;
<img src="https://img.shields.io/badge/-Matplotlib-FFF?style=for-the-badge&logo=matplotlib&logoColor=blue" title="Matplotlib" alt="Matplotlib" height="35"/>&nbsp;
<img src="https://img.shields.io/badge/Plotly_Express-white?logo=plotly&style=for-the-badge&logoColor=3F4F75" title="Plotly Express" alt="Plotly Express" height=35"/>&nbsp;
<img src="https://img.shields.io/badge/pingouin-white?style=for-the-badge" title="Pingouin" alt="Pingouin" height=35"/>&nbsp;
</div>


### 📂 Методы и подходы:

- A/B тестирование;
- Статистический анализ **(хи-квадрат, U-критерий Манна-Уитни, критерий Краскала-Уоллиса)**;
- Проверка гипотез о различиях между группами водителей;
- Анализ активности водителей в первые 30 дней после регистрации;
- Исследование связи оттока с разными характеристиками.

### 📊 В ходе проекта решены следующие задачи:

- Сформулированы гипотезы о факторах, влияющих на отток водителей;
- Проведена проверка связи оттока с городом с помощью критерия хи-квадрат (различия оказались статистически значимыми, p-value < 0.05);
- Проанализирована активность водителей в первые 30 дней с момента регистрации в зависимости от города с использованием критерия Краскала-Уоллиса (распределения оказались ненормальными);
- Проверена гипотеза о связи оттока с числом поездок в первые 30 дней с помощью U-критерия Манна-Уитни (уехавшие водители оказались менее активными, различия значимы);
- Выявлены ключевые факторы оттока, сформулированы рекомендации по удержанию водителей (улучшение программы лояльности, работа с неактивными водителями, исправление проблем на Android-приложении).

<hr>

### Описание данных:

[**Датасет**](https://github.com/ElenaAnalyst/product_analytics/blob/main/churn_analysis/churn.csv):

- `city` – город;
- `phone` – основное устройство, которое использует водитель;
- `signup_date` – дата регистрации аккаунта (YYYYMMDD);
- `last_trip_date` – дата последней поездки (YYYYMMDD);
- `avg_dist` – среднее расстояние (в милях) за поездку в первые 30 дней после регистрации;
- `avg_rating_by_driver` – средняя оценка поездок водителем;
- `avg_rating_of_driver` – средняя оценка поездок водителя;
- `surge_pct` – процент поездок, совершенных с множителем > 1 (кажется когда большая загруженность и тд);
- `avg_surge` – средний множитель всплеска за все поездки этого водителя;
- `trips_in_first_30_days` – количество поездок, которые совершил водитель в первые 30 дней после регистрации;
- `luxury_car_user` – TRUE, если пользователь в первые 30 дней использовал премиум-автомобиль;
- `weekday_pct` – процент поездок пользователя, совершенных в будние дни.
