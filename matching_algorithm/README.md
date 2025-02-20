## [А/B-тест алгоритма мэтчинга](https://github.com/ElenaAnalyst/product_analytics/blob/main/matching_algorithm/matching_algorithm.ipynb)
 Ознакомиться с файлом решения тут (нажать) ⤴️

### 🛠️ Стек:
<div>
<img src="https://img.shields.io/badge/python-white?logo=python&style=for-the-badge" title="Python" alt="Python" height=35"/>&nbsp;
<img src="https://img.shields.io/badge/pandas-white?logo=pandas&logoColor=blue&style=for-the-badge" title="Pandas" alt="Pandas" height="35"/>&nbsp;
<img src="https://img.shields.io/badge/-scipy.stats-FFF?style=for-the-badge&logo=scipy&logoColor=blue" title="scipy.stats" alt="scipy.stats" height="35"/>&nbsp;
<img src="https://img.shields.io/badge/-Seaborn-FFF?style=for-the-badge&logo=seaborn&logoColor=blue" title="Seaborn" alt="Seaborn" height="35"/>&nbsp;
<img src="https://img.shields.io/badge/-Matplotlib-FFF?style=for-the-badge&logo=matplotlib&logoColor=blue" title="Matplotlib" alt="Matplotlib" height="35"/>&nbsp;
<img src="https://img.shields.io/badge/pingouin-white?style=for-the-badge" title="Pingouin" alt="Pingouin" height=35"/>&nbsp;
</div>


### 📂 Методы и подходы:

- A/B тестирование;
- Статистический анализ (**t-критерий Уэлча, t-критерий Стьюдента**);
- Проверка гипотез о разнице в средней доле мэтчей и среднем количестве действий на пользователя;
- Оценка влияния нового алгоритма на ключевые метрики.

### 📊 В ходе проекта решены следующие задачи:

- Выбраны метрики для оценки качества сервиса: доля мэтчей и среднее количество действий на пользователя;
- Рассчитана средняя доля мэтчей на пользователя для контрольной (0) и тестовой (1) групп;
- Проведена проверка статистической значимости различий в средней доле мэтчей между группами с помощью t-критерия Уэлча. Нулевая гипотеза отклонена (p-value < 0.05), что говорит о значимых различиях;
- Оценено среднее количество действий на пользователя в контрольной и тестовой группах;
- Проведена проверка статистической значимости различий в количестве действий между группами с помощью t-критерия Стьюдента. Различия значимы (p-value < 0.05).

<hr>

**Сделан вывод о положительном влиянии нового алгоритма на ключевые метрики и рекомендовано его внедрение для всех пользователей.**
