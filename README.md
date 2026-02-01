## Анализ и визуализация больших данных. Машинное обучение на больших данных с использованием Apache Spark MLlib
#### Цель и задачи работы:
- Познакомиться с понятием «большие данные» и способами их обработки;
- Познакомиться с инструментом `Apache Spark` и возможностями, которые он предоставляет для обработки больших данных.
- Получить навыки выполнения разведочного анализа данных использованием `pyspark`.

#### Порядок выполнения работы:
1. Запустите конфигурацию `ds_mgpu_Hadoop3+spark_3_4` [скачать](http://95.131.149.21/moodle/mod/folder/view.php?id=1335) или запустить [файл](https://github.com/BosenkoTM/PySpark/blob/main/advanced_pyspark_for_exploratory_data_analysis_student.ipynb)  в colab.
2. Клонировать текущий репозиторий на компьютер в случае работы локально в Docker:
> `$ git clone https://github.com/BosenkoTM/PySpark.git`
3. Скачайте датасет, расположенный по адресу `https://drive.google.com/file/d/1yiAp1fFDy3wSqUR0X_btCZPtuczbLwCe/view?usp=drive_link` или [data](https://disk.yandex.ru/d/d80nsbNoP6F2vA). Распакуйте его и поместите файл `endomondoHR.json` в директорию `data` проекта (если директория отсутствует, создайте ее).
4. Не Colab: запустите докер-контейнер со средой разработки и инструментом `Apache Spark` и дождитесь завершения его работы.
> `$ sudo docker compose up`
  - Откройте браузер и перейдите по адресу: http://localhost:10000/lab
5. Откройте в браузере файл ноутбука с примером разведочного анализа [advanced_pyspark_for_exploratory_data_analysis_student.ipynb](https://github.com/BosenkoTM/PySpark/blob/main/advanced_pyspark_for_exploratory_data_analysis_student.ipynb). Изучите этот файл и запустите его.

**Обратите внимание:**
* Для сокращения расчетного времени можно обрабатывать только часть датасета;
* **Плагиат-работы не принимаются!**.


#### Список теоретических вопросов к отчету:
1. Фреймворк обработки больших данных `Apache Spark`, его назначение, функции и отличия от `Hadoop MapReduce`.
2. Понятие устойчивого распределенного набора данных (RDD). Понятие раздела RDD (partition). Способы создания RDD. Трансформации (transformations) и действия (actions). Кэширование (cache) данных в Spark.
3. RDD и PairRDD: понятие, назначение. Основные трансформации (transformations) и действия (actions) над ними.
4. Реализация концепции MapReduce в фреймворке Spark. Функции map, flatMap, mapValues, mapPartitions, reduce, reduceByKey.
5. Модели запуска Spark-приложений (YARN, Standalone, Kubernetes). Понятие драйвера (driver) и исполнителей (executors). Понятия задания (job), этапа (stage) и задачи (task). Модель ленивых вычислений (lazy) и ее применение в Spark. Понятие ориентированного ациклического графа (Directed Acyclic Graph, DAG).
6. Операция перемешивания данных (shuffle): причины возникновения, влияние на производительность. Класс Partitioner. Пути повышения производительности.
7. Понятие датафрейма в Spark. Основные операции над датафреймами. Скалярные функции, агрегирующие функции, оконные функции. Оптимизация запросов. Catalyst.
8. Клиентский (client) и кластерный (cluster) режимы работы Apache Spark.


#### Индивидуальные задания

Задания на образовательном портале [IT-Adaptive](https://envlab.ru/mod/assign/view.php?id=469)

#### Альтернативная работа(необязательно, в случае, если есть готовый проект)

В датасете должны быть представлены табличные данные, желательный объем — от нескольких гигабайт и выше. Датасеты можно выбрать на следующих ресурсах:

- [kaggle](https://www.kaggle.com/datasets) (для скачивания датасета требуется регистрация);

- [UC Irvine Machine Learning Repository](https://archive.ics.uci.edu/ml/index.php).

6. Выполните разведочный анализ датасета с определением: 
* типов признаков в датасете; 
* пропущенных значений и их устранением; 
* выбросов и их устранением; 
* расчетом статистических показателей признаков (средних, квартилей и т.д.); 
* визуализацией распределения наиболее важных признаков; 
* корреляций между признаками.

7. Сделайте выводы по работе.
8. Сохраните ноутбук с проведенным анализом в `GitHub / GitLab`, в котором опишите постановку задачи, описание датасета со ссылкой на него, проведенный разведовательный анализ и выводы.

**К отчету** следует представить ссылку на репозиторий `GitHub / GitLab/Gitverse` с выполненным разведочным анализом, а также быть готовым продемонстрировать работоспособность кода и пояснить спорные моменты.


#### Литература для подготовки к отчету:
1. Data Exploration // Learning Apache Spark with Python [Электронный  ресурс] / W. Feng. - [2021]. - Режим доступа : https://runawayhorse001.github.io/LearningApacheSpark/exploration.html (дата обращ. 10.03.2025).
2. Advanced Pyspark for Exploratory Data Analysis [Электронный  ресурс]. – [2022]. – Режим доступа : https://www.kaggle.com/code/tientd95/advanced-pyspark-for-exploratory-data-analysis (дата обращ. 10.03.2025). 
3. Exploratory Data Analysis (EDA) with PySpark on Databricks [Электронный  ресурс]. – [2020]. – Режим доступа : https://towardsdatascience.com/exploratory-data-analysis-eda-with-pyspark-on-databricks-e8d6529626b1 (дата обращ. 10.03.2025).
4. Exploratory data analysis with pySpark [Электронный  ресурс]. – [2020]. – Режим доступа : https://github.com/BosenkoTM/PySpark/tree/main/pySpark_tutorial-master (дата обращ. 10.03.2025).
5. Официальный сайт Apache Spark [Электронный  ресурс]. – [2022]. – Режим доступа : https://spark.apache.org/ (дата обращ. 10.03.2025).
