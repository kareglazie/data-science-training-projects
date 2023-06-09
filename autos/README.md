В этом проекте мы обучили модель для быстрого предсказания цены на подержанные автомобили. Важно было не только добиться определенного качества (значения метрики RMSE не ниже 2500), но и выбрать наиболее оптимальную модель с точки зрения скорости обучения и предсказания, поскольку она будет использоваться в приложении (пользователи вводят данные об автомобиле и получают на выходе цену).

- Была проведена предобработка данных (удалены не значимые для модели признаки, заполнены пропуски, обработаны аномальные значения).
- Были обучены три модели — решающее дерево, случайный лес и LightGBM. Также проверена адекватность моделей с помощью дамми-модели.
- По результатам исследования была выбрана модель LightGBM — она показала оптимальные результаты с точки зрения соотношения показателей качество/скорость.
- Указанная модель была проверена на тестовой выборке и показала хорошее значение метрики RMSE.

**Инструменты**

- pandas
- numpy
- matplotlib
- sklearn
- lightgbm
