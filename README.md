<p align="center">
  <img src="data-pipeline.gif" alt="Анимация пайплайна данных: S3, Spark, Greenplum и Airflow" width="100%">
</p>

<h1 align="center">Привет, меня зовут Владислав! 👋</h1>
<h3 align="center">Инженер данных · Data Engineer</h3>

## 👨‍💻 Обо мне

Учусь в Воронежском государственном техническом университете (ВГТУ) по направлению «Прикладная информатика». В процессе обучения понял, что меня привлекает инженерия данных: нравится упорядочивать информацию и выстраивать процессы, которые делают её полезной и доступной для других.

Прошёл курс по Data Engineering от **karpov.courses** и продолжаю развиваться в этой сфере. Читаю документацию, решаю задачи на LeetCode и Codewars, использую ИИ для разбора сложных тем и анализа своих решений. Ищу команду, в которой смогу применять полученные знания, учиться у опытных коллег и приносить пользу общему делу.

В свободное время слежу за баскетболом, теннисом и футболом, посещаю тренажёрный зал. Люблю поддерживать в порядке и физическую форму, и данные.

## 🛠️ Мой стек

**Языки и обработка данных**

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-315B8E?style=for-the-badge)
![pandas](https://img.shields.io/badge/pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Apache Spark](https://img.shields.io/badge/Apache_Spark-E25A1C?style=for-the-badge&logo=apachespark&logoColor=white)

**Базы данных и оркестрация**

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![ClickHouse](https://img.shields.io/badge/ClickHouse-FFCC01?style=for-the-badge&logo=clickhouse&logoColor=black)
![Apache Airflow](https://img.shields.io/badge/Apache_Airflow-017CEE?style=for-the-badge&logo=apacheairflow&logoColor=white)

**Инструменты**

![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=for-the-badge&logo=gnubash&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![GitLab](https://img.shields.io/badge/GitLab-FC6D26?style=for-the-badge&logo=gitlab&logoColor=white)

**Подходы:** ETL, DWH, ER-диаграммы.

## 📖 Мой проект

### Витрина данных для маркетплейса KarpovZone

**Учебный проект курса Data Engineering от karpov.courses.**

**Цель:** подготовить витрину с агрегированными метриками по товарам и категориям для аналитиков маркетплейса.

**Стек проекта:** Python, PySpark, SQL, Apache Airflow, Greenplum, S3, Kubernetes, GitLab.

**Что сделал:**

- Разработал Spark-задачу для чтения данных из S3, обогащения дополнительными полями и записи результата в отдельную папку S3.
- Собрал DAG в Airflow: запуск Spark-задачи в Kubernetes через `SparkKubernetesOperator`, ожидание её завершения через `SparkKubernetesSensor` и выполнение SQL-запросов через три `SQLExecuteQueryOperator`.
- Подготовил SQL-запросы для создания внешних таблиц и представлений в Greenplum, обеспечив доступ к обработанным данным в S3.

**Результат:** собрал единый пайплайн от исходных данных в озере до аналитической витрины в Greenplum. На практике связал хранение в S3, распределённую обработку в Spark и оркестрацию в Airflow.

<!-- После публикации кода добавь сюда ссылку на репозиторий проекта. -->
