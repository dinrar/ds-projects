<p align="center"> Проекты по Data Science </p align="center">

[Сертификат о прохождении курса DS](https://github.com/dinrar/ds-projects/tree/main/_certificates)

| **Проект** | **Задание** |**Что сделано** | **Библиотеки** |
| - | :- |:-|:-|
| [01. Исследование данных о компьютерных играх (EDA, A/B-test)](https://github.com/dinrar/ds-projects/tree/main/video_games_research) | Определить признаки, по которым можно выявить потенциально популярную видеоигру. Предоставлены исторические данные о продажах игр, оценках пользователей и экспертов, жанре и платформах, для которых они публиковались, за период до 2015 года (предсказание необходимо сделать на 2016 год). Дополнительно необходимо проверить 2 гипотезы: средние пользовательские рейтинги платформ Xbox One и PC одинаковые; средние пользовательские рейтинги жанров Action и Sports разные. | Выполнены подготовка и исследовательский анализ данных; определены признаки, по которым можно определить потенциально успешную игру; проверены сформулированные в задании заказчика; даны рекомендации, которые стоит учесть заказчику при планировании рекламной кампании. | scipy, math, numpy, pandas|
| [02. Прогнозирование заказов такси (time-series data)](https://github.com/dinrar/ds-projects/tree/main/taxi_demand_prediction) | Предсказать количество заказов такси на час вперед с заданной метрикой *RMSE*. Предоставлены данные о количестве заказов за одинаковые периоды времени. | Выполнен анализ данных, обучены 5 моделей машинного обучения: дерево решений, случайный лес, линейная регрессия, ElasticNet, градиентный бустинг. Лучший результат получен с использованием модели градиентного бустинга. | matplotlib, sklearn, statsmodels.tsa.seasonal, catboost, numpy, pandas, seaborn, shap |
| [03. Определение токсичных комментариев (NLP)](https://github.com/dinrar/ds-projects/tree/main/toxic_comments_detection) | Разработать инструмент для автоматического выявления токсичных правок с заданной метрикой *f1*. Предоставлен набор комментариев с разметкой токсичности. | Выполнен анализ данных, подготовлены эмбеддинги из части текстов исходного корпуса, обучены 3 модели машинного обучения: дерево решений, случайный лес, логистическая регрессия. Лучший результат получен для модели случайного леса. | sklearn, tqdm, BERT (RoBERTa), numpy, pandas, torch |
| [04. Определение возраста покупателей по фото (CV)](https://github.com/dinrar/ds-projects/tree/main/age_determining_by_photo) | Определить возраст по фотографии с заданной метрикой *MAE*. Предоставлен набор фотографий с лицами людей разного возраста. | Выполнен анализ данных, обучена сверточная нейронная сеть ResNet-50. | pandas, keras |
| [05. Предсказание температуры в плавильном ковше](https://github.com/dinrar/ds-projects/tree/main/melting_ladle_temperature) | Предсказать температуру в плавильном ковше с заданной метрикой *MAE*. Предоставлены данные о параметрах работы нагревательного устройства (электрической дуги), материалах, поступающих в ковш (сыпучие, проволочные, газ), температуре в ковше в разные моменты времени. | Выполнен анализ и обработка данных, сгенерированы новые признаки, обучены 3 модели машинного обучения (линейная регрессия, случайный лес, градиентный бустинг). Лучший результат получен для модели градиентного бустинга (CatBoost). | catboost, numpy, optuna, pandas, pandas_profiling, seaborn, shap, sklearn, matplotlib |

**Dinar Suleymanov**
dinrar@gmail.com