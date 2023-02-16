<p align="center"> Проекты по Data Science </p align="center">

Рекомендуется смотреть через [External viewer](https://nbviewer.jupyter.org/github/ArtyKrafty/Data_science_projects/tree/9d86c5514664c670c928edbb1eb0f857e62e4e5e/) или [Google Collab](https://colab.research.google.com/)

[Сертификаты о прохождении курсов](https://github.com/dinrar/ds-projects/tree/main/_certificates)
__________________________________________________________________________________________________________________________


| **Проект** | **Описание** |**Что сделано** | **Библиотеки** |
| -------------------- | :--------------------- |:---------------------------|:---------------------------|
| [01. Исследование данных о компьютерных играх](https://github.com/dinrar/ds-projects/tree/main/video_games_research%20(EDA%2C%20A_B-test)) | Заказчиком выступает интернет-магазин, занимающийся продажей видеоигр - для лучшего планирования рекламной кампании необходимо определить признаки, по которым можно выявить потенциально популярный продукт. Информация о продажах игр, оценках пользователей и экспертов, жанре и платформах, для которых они публиковались, собрана в файле `games.csv`. Дополнительно необходимо проверить 2 гипотезы, сформулированные заказчиком: средние пользовательские рейтинги платформ Xbox One и PC одинаковые; средние пользовательские рейтинги жанров Action и Sports разные. | Выполнены подготовка и исследовательский анализ данных; определены признаки, по которым можно определить потенциально успешную игру; проверены сформулированные в задании заказчика; даны рекомендации, которые стоит учесть заказчику при планировании рекламной компании. | scipy, math, numpy, pandas|
| [02. Прогнозирование заказов такси](https://github.com/dinrar/ds-projects/tree/main/taxi_demand_prediction%20(Time-Series%20Data)) | Компания, предоставляющая услуги такси, планирует привлекать больше водителей в период пиковой нагрузки для обслуживания клиентов, находящихся в аэропорту, для чего необходимо разработать инструмент, способный предсказывать количество заказов на час вперед с метрикой *RMSE* не больше 48. Предоставленные заказчиком данные о количестве заказов за периоды по 10 минут хранятся в файле `taxi.csv`. | Выполнен анализ данных, обучены 5 моделей машинного обучения: дерево решений, случайный лес, линейная регрессия, ElasticNet, градиентный бустинг. Лучший результат получен с использованием модели градиентного бустинга. Значение *RMSE* на тестовой выборке составило 41,8. | matplotlib, sklearn, statsmodels.tsa.seasonal, catboost, numpy, pandas, seaborn, shap |
| [03. Определение токсичных комментариев](https://github.com/dinrar/ds-projects/tree/main/taxi_demand_prediction%20(Time-Series%20Data)) | Интернет-магазин планирует добавление на сайт возможности добавления и редактирования описаний товаров по аналогии с вики-сообществами. Помимо прочего, необходимо разработать инструмент для автоматического выявления токсичных правок, которые должны отправляться на проверку модератору. Метрика *f1* работы данного инструмента должна быть не меньше 0,75. Заказчиком предоставлен набор комментариев с разметкой токсичности правок. | Выполнен анализ данных, подготовлены эмбеддинги из части текстов исходного корпуса, обучены 3 модели машинного обучения: дерево решений, случайный лес, логистическая регрессия. Лучший результат получен для модели случайного леса. На тестовой выборке *f1* составило 0,77. | sklearn, tqdm, BERT (RoBERTa), numpy, pandas, torch |
| [03. Определение токсичных комментариев](https://github.com/dinrar/ds-projects/tree/main/toxic_comments_detection%20(NLP)) | Интернет-магазин планирует добавление на сайт возможности добавления и редактирования описаний товаров по аналогии с вики-сообществами. Помимо прочего, необходимо разработать инструмент для автоматического выявления токсичных правок, которые должны отправляться на проверку модератору. Метрика *f1* работы данного инструмента должна быть не меньше 0,75. Заказчиком предоставлен набор комментариев с разметкой токсичности правок. | Выполнен анализ данных, подготовлены эмбеддинги из части текстов исходного корпуса, обучены 3 модели машинного обучения: дерево решений, случайный лес, логистическая регрессия. Лучший результат получен для модели случайного леса. На тестовой выборке *f1* составило 0,77. | sklearn, tqdm, BERT (RoBERTa), numpy, pandas, torch |
| [04. Определение возраста покупателей по фото](https://github.com/dinrar/ds-projects/tree/main/age_determining_by_photo%20(CV)) | Сетевой супермаркет внедряет систему компьютерного зрения для определения возраста покупателей с целевой метрикой *MAE* не хуже 8 лет. Заказчиком предоставлен набор из 7591 фотографий, на которых изображены люди в возрасте от 1 до 100 лет. | Выполнен анализ данных, обучена сверточная нейронная сеть ResNet-50. Итоговое значение метрики *MAE* составило 7,6 года. | pandas, keras |
| [05. Предсказание температуры в плавильном ковше](https://github.com/dinrar/ds-projects/tree/main/melting_ladle_temperature) | Металлургическому заводу требуется предсказать температуру в плавильном ковше с метрикой *MAE* не хуже 6,8 °C. Предоставлены 7 таблиц с информацией о параметрах работы нагревательного устройства (электрической дуги), материалах, поступающих в ковш (сыпучие, проволочные, газ), температуре в ковше в разные моменты времени. | выполнен анализ и обработка данных, сгенерированы новые признаки, обучены 3 модели машинного обучения (линейная регрессия, случайный лес, градиентный бустинг). Лучший результат получен для модели градиентного бустинга (CatBoost). Значение *MAE* на тестовой выборке составило 5,3 °C. | catboost, numpy, optuna, pandas, pandas_profiling, seaborn, shap, sklearn, matplotlib |



**Dinar Suleymanov**
dinrar@gmail.com