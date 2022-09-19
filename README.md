# АНАЛИЗ ДАННЫХ И ИСКУССТВЕННЫЙ ИНТЕЛЛЕКТ [in GameDev]
Отчет по лабораторной работе #1 выполнил(а):
- Амбрушкевич Артем Антонович
- РИ-211002
Отметка о выполнении заданий (заполняется студентом):

| Задание | Выполнение | Баллы |
| ------ | ------ | ------ |
| Задание 1 | * | 60 |
| Задание 2 | * | 20 |
| Задание 3 | # | 20 |

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
Ознакомиться с основными операторами зыка Python на примере реализации линейной регрессии.

## Задание 1
### Пошагово выполнить каждый пункт раздела "ход работы" с описанием и примерами реализации задач
Ход работы:
Написать программы Hello World на Python и Unity
- На Python
![Отчет hello world in python](https://user-images.githubusercontent.com/97295011/190987455-a064be6b-3d9a-4785-a75b-9ad9bf680b3e.jpg)
- На Unity
![Отчет hello world in unity](https://user-images.githubusercontent.com/97295011/190987514-37308dae-6700-42c5-80ed-062496f1e8a1.jpg)



## Задание 2
### В разделе "ход работы" пошагово выполнить каждый пункт с описанием и примером реализации задачи по теме лабораторной работы
- 1. Производим подготовку данных для работы с алгоритмом линейной регрессии. 10 видов данных были установлены случайным образом, и данные находились в линейной зависимости. Данные преобразуются в формат массива, чтобы их можно было вычислить напрямую при использовании умножения и сложения.
![1](https://user-images.githubusercontent.com/97295011/190991378-2953d397-9561-42e5-858e-72723fde6670.JPG)

- 2. Определяем связанные функции. Функция модели: определяет модель линейной регрессии wx+b. Функция потерь: функция потерь среднеквадратичной ошибки. Функция оптимизации: метод градиентного спуска для нахождени частных производных w и b.
![2](https://user-images.githubusercontent.com/97295011/190991975-2fbba71b-f569-463a-a783-cb9ca5f8701e.JPG)

- 3. Начинаем итерацию

     Шаг 1 Инициализация и модель итеративной оптимизации
     
     ![3 1](https://user-images.githubusercontent.com/97295011/190993809-ba0ca821-e67d-4745-a0b5-6c0404e79d6d.JPG)
     
     Шаг 2 На второй итерации отображаются значения  параметров, значения потерь и эффекты визуализации после итерации
     
     ![3 2](https://user-images.githubusercontent.com/97295011/190994146-509c0933-f210-4f78-81d3-45d1d1b83314.JPG)
     
     Шаг 3 Третья итерация показывает значения  параметров, значения потерь и визуализацию после итерации
     
     ![3 3](https://user-images.githubusercontent.com/97295011/190994371-8aca5803-ad2f-4caf-a114-6fa97c30e58e.JPG)
     
     Шаг 4 На четвертой итерации отображаются значения параметров, значения потерь и эффекты визуализации
     
     ![3 4](https://user-images.githubusercontent.com/97295011/190994535-94e5afad-78e7-414b-b1ba-cc459032845c.JPG)
     
     Шаг 5 Пятая итерация показывает значение параметра, значение потерь и эффект визуализации после итерации
     
     ![3 5](https://user-images.githubusercontent.com/97295011/190994628-a1f50f44-6558-493e-a267-8475c9578eb1.JPG)
     
     Шаг 6 10000-я итерация, показывающая значения параметров, потери и визуализацию после итерации
     
     ![3 6](https://user-images.githubusercontent.com/97295011/190994729-5baab077-554c-430f-aad8-88089008a2d9.JPG)
     

## Задание 3
### Какова роль параметра Lr? Ответьте на вопрос, приведите пример выполнения кода, который подтверждает ваш ответ. В качестве эксперимента можете изменить значение параметра.

- Перечисленные в этом туториале действия могут быть выполнены запуском на исполнение скрипт-файла, доступного [в репозитории](https://github.com/Den1sovDm1triy/hfss-scripting/blob/main/ScreatingSphereInAEDT.py).
- Для запуска скрипт-файла откройте Ansys Electronics Desktop. Перейдите во вкладку [Automation] - [Run Script] - [Выберите файл с именем ScreatingSphereInAEDT.py из репозитория].

```py

import ScriptEnv
ScriptEnv.Initialize("Ansoft.ElectronicsDesktop")
oDesktop.RestoreWindow()
oProject = oDesktop.NewProject()
oProject.Rename("C:/Users/denisov.dv/Documents/Ansoft/SphereDIffraction.aedt", True)
oProject.InsertDesign("HFSS", "HFSSDesign1", "HFSS Terminal Network", "")
oDesign = oProject.SetActiveDesign("HFSSDesign1")
oEditor = oDesign.SetActiveEditor("3D Modeler")
oEditor.CreateSphere(
	[
		"NAME:SphereParameters",
		"XCenter:="		, "0mm",
		"YCenter:="		, "0mm",
		"ZCenter:="		, "0mm",
		"Radius:="		, "1.0770329614269mm"
	], 
)

```

## Выводы

Абзац умных слов о том, что было сделано и что было узнано.

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
