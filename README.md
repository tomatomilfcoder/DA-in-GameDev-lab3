# АНАЛИЗ ДАННЫХ И ИСКУССТВЕННЫЙ ИНТЕЛЛЕКТ [in GameDev]
Отчет по лабораторной работе #3 выполнил(а):
- Русакова Анна Алексеевна
- РИ-230947
Отметка о выполнении заданий (заполняется студентом):

| Задание | Выполнение | Баллы |
| ------ | ------ | ------ |
| Задание 1 | * |  |
| Задание 2 | * |  |
| Задание 3 | * |  |

знак "*" - задание выполнено; знак "#" - задание не выполнено;

Работу проверили:
- к.т.н., доцент Денисов Д.В.
- к.э.н., доцент Панов М.А.
- ст. преп., Фадеев В.О.

[![N|Solid](https://cldup.com/dTxpPi9lDf.thumb.png)](https://nodesource.com/products/nsolid)

[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://travis-ci.org/joemccann/dillinger)

Структура отчета

- Данные о работе: название работы, фио, группа, выполненные задания.
- Цель работы.
- Задание 1.
- Код реализации выполнения задания. Визуализация результатов выполнения (если применимо).
- Задание 2.
- Код реализации выполнения задания. Визуализация результатов выполнения (если применимо).
- Задание 3.
- Код реализации выполнения задания. Визуализация результатов выполнения (если применимо).
- Выводы.
- ✨Magic ✨

## Цель работы
Разработать оптимальный баланс изменения сложности для десяти уровней игры Dragon Picker.


## Задание 1. Начало работы с прототипом
### Ознакомьтесь с презентацией третьей лекции, оцените структуры игры Dragon Picker. Скачайте и ознакомьтесь с прототипом игры Dragon Picker на движке Unity. Запустите игровую сцену, проанализируйте движение дракона: Какие переменные влияют на движение дракона на сцене? Укажите эти переменные. Какие переменные влияют на сложность игры на сцене? Укажите эти переменные.

### Ход работы:

- Проанализировать движение дракона.
  На движение дракона влияют параметры Speed, Left Right Distance и Chance Direction (вероятность досрочной смены направления движения)
- Проанализировать сложность игры.
  На сложность игры влияют Speed, Time Between Egg Drops (промежуток времени между спавном яиц), Chance Direction, Num Energy Shield (количество энергетических щитов, которыми игром ловит яйца) и Energy Shield Radius (радиус щита).


## Задание 2. Начало работы с шаблоном google-таблицы для балансировки игры
### Ознакомьтесь с презентацией третьей лекции, оцените структуры шаблона таблицы для балансировки. Отметьте, как может быть использован шаблон таблицы для визуализации изменения уровней сложности в игре Dragon Picker.

### Ход работы:

- Ознакомиться с презентацией третьей лекции.
  Шаблон таблицы можно использовать для наблюдения за тем, как изменяются переменные баланса в зависимости от каждого уровня, с помощью визуализации различными графиками (гистограммы, диаграммы и т.д.)


## Задание 3. Задания к работе

### Задание 1. Предложите вариант изменения найденных переменных для 10 уровней в игре

#### Ход работы:

- Определить, как менять параметры для сбалансированного роста сложности.
  Я решила менять 4 параметра: Speed, Time Between Egg Drops, Num Energy Shield и Energy Shield Radius. Для первых двух задала коэффициенты 1,2 и 0,9 соответственно, количество щитов уменьшается на 1 через каждые 3 уровня, а насчёт решила, что он будет одинаковый до последнего уровня (1,5 -> 1), чтобы он ощущался непропорционально сложнее предыдущих (он же все-таки последний), но не сильно.

![image](https://github.com/user-attachments/assets/4a7d5e46-4a09-41bb-a59a-d2c123e16f17)


### Задание 2. Создайте 10 сцен на Unity с изменяющимся уровнем сложности.

#### Ход работы:

- Склонировать сцену 10 раз.

![image](https://github.com/user-attachments/assets/5e60ca99-04fe-49fa-bd94-d6b0b4af4a14)

- Заполнить параметры.

| Сцена | Параметры |
| ------ | ------ |
| 1 | ![image](https://github.com/user-attachments/assets/8223072b-0ea6-4799-90c3-37b945c4546d) ![image](https://github.com/user-attachments/assets/5722f26a-41be-4929-a71f-0d92f7fb4300) |
| 2 | ![image](https://github.com/user-attachments/assets/19f98460-b717-4080-bb22-ebe1c9d0b76c) ![image](https://github.com/user-attachments/assets/5722f26a-41be-4929-a71f-0d92f7fb4300) |
| 3 | ![image](https://github.com/user-attachments/assets/e83de0de-27d7-41be-9be6-b29d86d28cee) ![image](https://github.com/user-attachments/assets/5722f26a-41be-4929-a71f-0d92f7fb4300) |
| 4 | ![image](https://github.com/user-attachments/assets/643482c8-49ef-461d-9d40-e52e167eea6b) ![image](https://github.com/user-attachments/assets/5722f26a-41be-4929-a71f-0d92f7fb4300) |
| 5 | ![image](https://github.com/user-attachments/assets/6f5b090c-e382-4bdb-8619-d37895c7fca7) ![image](https://github.com/user-attachments/assets/d84d4b63-5565-491b-89ba-88838b1d9f62) |
| 6 | ![image](https://github.com/user-attachments/assets/2e8fb5ae-1281-4b0a-88b0-6443bb9f396f) ![image](https://github.com/user-attachments/assets/d84d4b63-5565-491b-89ba-88838b1d9f62) |
| 7 | ![image](https://github.com/user-attachments/assets/18109d4b-e348-4e88-94bf-d78b8d03895a) ![image](https://github.com/user-attachments/assets/d84d4b63-5565-491b-89ba-88838b1d9f62) |
| 8 | ![image](https://github.com/user-attachments/assets/c0cae7d8-30b0-4472-84cb-1ec715cc784a) ![image](https://github.com/user-attachments/assets/d84d4b63-5565-491b-89ba-88838b1d9f62) |
| 9 | ![image](https://github.com/user-attachments/assets/a14382cf-fb9b-44c4-85a2-2a1fedb5023e) ![image](https://github.com/user-attachments/assets/52279f4f-1424-4098-82c1-1451f7d8cb42) |
| 10 | ![image](https://github.com/user-attachments/assets/a0bd5821-92fb-4c7d-9f48-04a56ca34671) ![image](https://github.com/user-attachments/assets/52279f4f-1424-4098-82c1-1451f7d8cb42) |


### Задание 3 не выполнено


## Выводы
Я научилась работать с параметрами баланса, визуализировать их и применять изменения переменных в Unity.


| Plugin | README |
| ------ | ------ |
| Dropbox | [plugins/dropbox/README.md][PlDb] |
| GitHub | [plugins/github/README.md][PlGh] |
| Google Drive | [plugins/googledrive/README.md][PlGd] |
| OneDrive | [plugins/onedrive/README.md][PlOd] |
| Medium | [plugins/medium/README.md][PlMe] |
| Google Analytics | [plugins/googleanalytics/README.md][PlGa] |

## Powered by

**BigDigital Team: Denisov | Fadeev | Panov**
