### Описание этапа обработки данных

Столбец floor: удалили данные, где были строковые значения типа "подвал", "первый" и т.д., т.к. их было меньше процента. Столбец floor перекодировали в категориальный признак с несколькими значениями: first/basement/higher_floor/multy_level и unknown для пропущенных значений.

Столбцы: reform_house_population_1000', 'reform_house_population_500','reform_mean_floor_count_1000', 'reform_mean_floor_count_500','reform_mean_year_building_1000', 'reform_mean_year_building_500', в них пропуски заполнили средними по городу/региону.

Дополнительные данные: добавили ставку рефинансирования. (ссылка: https://www.klerk.ru/tools/refinancing/)

### Описание процесса обучения и получения результата
Обучали модель только на строках, где price_type = 1.
Лучшая метрика получилась у градиентного бустинга (catboostregressor) c depth = 12, iterations = 1200
Получили score = 1.3602185953742985	
С учётом корректирующего эмпирического коэффициента 0,9:
test_predict_corrected = test_predict*0.9
