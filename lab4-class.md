# Лабораторная работа №4: Классификация в sklearn + метрики классификации

[Лекция](ML-1-class-metrics.ipynb)

1. Многоклассовая классификация
    1. На любом датасете продемонстрировать многоклассовую классификацию с помощью ЛЮБОГО алгоритма. Оценить accuracy.
    2. То же самое с использованием кросс-валидации
    3. Поиграться с гиперпараметром, связанным со сложностью модели (в случае kNN — k_neighbours) и построить график accuracy для train set и test_set для разных значений гиперпараметра (в лекции есть пример построения подобного графика для kNN и датасета cancer, но можно строить как угодно такой график)
    4. Построить confusion matrix ([пример](https://scikit-learn.org/stable/auto_examples/model_selection/plot_confusion_matrix.html)): ```
confusion_scores = sklearn.metrics.confusion_matrix( y_test, y_pred )
confusion_df = pd.DataFrame( confusion_scores, columns = iris.target_names, index = iris.target_names )
sns.heatmap( confusion_df, annot = True  )
```

2. На любом (но уже другом, бинарном) датасете продемонстрировать бинарную классификацию (можно использовать любой алгоритм), посчитать метрики: accuracy, precision, recall, f-measure, а также составить classification_report

Замечание: в обоих задачах (бинарной и многоклассовой классификации) попробовать также вариант с предварительной нормализацией признаков (`StandardScaler`или `MinMaxScaler`). Оценить метрики качества в случае с нормализованными признаками и ненормализованными.
