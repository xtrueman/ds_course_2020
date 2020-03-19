# Лабораторная работа №6: Catboost

Вначале надо установить нужные библиотеки:
```
pip3 install catboost shap ipywidgets
jupyter nbextension enable --py widgetsnbextension
```

Туториал по Catboost:
https://github.com/catboost/tutorials/blob/master/ru/ml_session_2018_tutorial_ru.ipynb

Мастеркласс по классификации при помощи Catboost:
https://www.youtube.com/watch?v=xl1fwCza9C8

1. Применить классификатор `CatBoostClassifier` к вашему датасету (бинарная или multiclass классификация по желанию).  
Можно работать на тех же данных, что и в предыдущей Л.Р.: в этом случае сравнить с результатами лучшего классификатора из предыдущей работы.  
Вывести итерацию с наилучшим значением AUC (для бинарной классификации) или наилучшим значением Logloss.  
Вывести значения метрик качества классификации на тестовых данных (accuracy и precision / recall / AUC, если применимо).

    Примеры классификатора: см. https://github.com/catboost/tutorials/blob/master/classification/classification_tutorial.ipynb

2. Применить регрессию CatBoostRegressor к вашему датасету.
Вывести номер итерации с значения метрик (MAE и MSE) для наилучшей итерации.

    Пример использования регрессора тут: https://github.com/catboost/tutorials/blob/master/model_analysis/shap_values_tutorial.ipynb

3. Для бинарного классификатора на основе CatBoostClassifier построить кривые PRC и ROC. Вычислить значения PRC-AUC и ROC-AUC.

    Примеры построения ROC-кривой есть в `classification_tutorial.ipynb`

В случае проблем с установкой / использованием CatBoost можно заменить его на xgboost.
