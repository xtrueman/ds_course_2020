# Курс "Инструменты анализа данных" 2020

© Валерий Студенников

Нам понадобится Python 3 и дополнительные библиотеки:

```
pip3 install -U numpy
pip3 install -U pandas
pip3 install -U sklearn
pip3 install -U matplotlib
```

Кому нужно вдруг подтянуть Python, рекомендую ресурс http://pythontutor.ru/,
где краткая теория и можно быстро и весело порешать несложные задачки онлайн.
На занятиях будем исходить из того, что Python не представляет сложностей )

## Варианты работы с блокнотами Jupyter:

### Jupyter-сервер

Классика жанра: запускаете Jupyter-web-сервер где-то у себя:

```
pip3 install -U jupyter

jupyter-notebook
```
Затем открываем в браузере http://localhost:8888/

### Приложение nteract

Оболочка для Jupyter Notebook на десктопе (под разные ОС):

https://nteract.io/

### Jupyter Lab

Расширенный вариант Jupyter Notebook блекджеком и табами.
https://jupyterlab.readthedocs.io/

Тоже запускается как web-сервер:
```
pip3 install jupyterlab

jupyter lab
```

Затем открываем в браузере http://localhost:8888/

### Облачные блокноты

* Бесплатный хостинг Juputer-блокнотов от Google:  
    https://colab.research.google.com/
* Другие варианты облачных Jupyter-блокнотов:  
    https://www.dataschool.io/cloud-services-for-jupyter-notebook/

## Требования к оформлению лабораторных работ:

1. Присылать ответы в jupyter-блокнотах со следующим названием файла:
`номерзадания-названиезадания-вашеимяфамалия.ipynb`, например, `01-numpy-ivan_ivanov.ipynb`

    В заголовке самого блокнота (в самой первой ячейке) также — название задания и ФИО автора.

2. Все ячейки, требующие вычисления, должны быть вычислены и в присылаемом блокноте должен содержаться вывод ячеек. Пустой блокнот с очищенным выводом ячеек не принимается!

3. Внутри в markdown-ячейках обязательно дублируете условие задачи в виде оглавления, каждую подзадачу предваряете markdown-ячейкой с описанием подзадачи.

4. Очень желательны комментарии к коду, которые объясняют, что делает тот или иной фрагмент. Нам за reverse engeneering не доплачивают ))

5. Код по-возможности структурируйте в небольший логические блоки, каждый в своей ячейке, чтобы легко было его понять. Выводите в блокнот промежуточные результаты. Вам же будет удобнее.

6. Если в работе используется какой-то датасет — ссылку на место, откуда его взяли и на описание длатсета. Хорошо рядом с загрузкой датасета кратко продублируете описание датасета — что это такое и о чём.
Это важно, например, для правильной трактовки признаков, например, чтобы отделить категоривальные признаки от вещественных.


## Полезные ссылки

* [Синтаксис markdown для Jupyter](https://sourceforge.net/p/jupiter/wiki/markdown_syntax/)
* [NumPy cheatsheet](https://s3.amazonaws.com/assets.datacamp.com/blog_assets/Numpy_Python_Cheat_Sheet.pdf)

## Датасеты:

Откуда брать датасеты для работ?

* [Встроенные датасеты в sklern](https://scikit-learn.org/stable/datasets/index.html)
* [Google-поиск по датасетам](https://datasetsearch.research.google.com/) 

Репозитории с датасетами: 
* [Kaggle](https://www.kaggle.com/datasets)
    ([как начать работу в Kaggle: руководство для новичков в Data Science](https://habr.com/ru/post/248395/))
* [Материалы с курса OpenDataScience](https://nbviewer.jupyter.org/github/Yorko/mlcourse.ai/tree/master/data/) [или тут]( https://github.com/Yorko/mlcourse.ai/tree/master/data/)
* [Датасеты университета Калифорнии](https://archive.ics.uci.edu/ml/datasets.php)
* [Учебные датасеты для R](https://vincentarelbundock.github.io/Rdatasets/datasets.html)
* [Датасеты от FiveThirtyEight](https://data.fivethirtyeight.com/)
* [Подборка на habr](https://habr.com/ru/post/452740/)
* [Ещё подборка](https://towardsai.net/p/machine-learning/best-free-datasets-for-machine-learning-and-data-science/stanfordai/3451/)
* [И ещё подборка](https://towardsdatascience.com/top-sources-for-machine-learning-datasets-bb6d0dc3378b)

Всяческие открытые данные: 
* [Списки источников открытых данных от Яндекса](https://yandex.ru/promo/oda/useful)
* [Портал открытых данных Российской Федерации](https://data.gov.ru/). Так себе источник, но может кто-то что-то там для себя найдёт
* [Портал открытых данных правительства Москвы](https://data.mos.ru/opendata). Правда с числовыми полями там не очень, зато много категориальных, можно потренироваться со всякими группировками. На лекции с pandas категориальные группировки нам как раз понадобятся.
* [Открытые данные Сбербанка](https://www.sberbank.com/ru/analytics/opendata)
* [Отктытые данные минфина](https://www.minfin.ru/opendata/)
* [Отктытые данные минкульта](https://opendata.mkrf.ru/opendata/)

## Лабораторные работы:

1. [NumPy](lab1-numpy.md)
2. [Pandas](lab2-pandas.md)
3. [Визуализация данных](lab3-visual.md)
