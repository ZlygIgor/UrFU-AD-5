# АНАЛИЗ ДАННЫХ И ИСКУССТВЕННЫЙ ИНТЕЛЛЕКТ [in GameDev]
Отчет по лабораторной работе #5 выполнил(а):
- Злыгостев Игорь Сергеевич
- РИ221001
Отметка о выполнении заданий (заполняется студентом):

| Задание | Выполнение | Баллы |
| ------ | ------ | ------ |
| Задание 1 | * | 60 |
| Задание 2 | * | 20 |
| Задание 3 | * | 20 |

знак "*" - задание выполнено; знак "#" - задание не выполнено;

Работу проверили:
- к.т.н., доцент Денисов Д.В.
- к.э.н., доцент Панов М.А.
- ст. преп., Фадеев В.О.

[![N|Solid](https://cldup.com/dTxpPi9lDf.thumb.png)](https://nodesource.com/products/nsolid)

[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://travis-ci.org/joemccann/dillinger)

## Цель работы
познакомиться с программными средствами для создания системы машинного обучения и ее интеграции в Unity.

## Задание 1
### Задание 1 - Найдите внутри C# скрипта “коэффициент корреляции ” и сделать выводы о том, как он влияет на обучение модели.

коэффицент корреляции влияет на совпадение между данными и моделью

## Задание 2
### Задание 2 - Изменить параметры файла yaml-агента и определить какие параметры и как влияют на обучение модели. Привести описание не менее трех параметров.

epsilon (Изменяется в пределах 0.1-0.3)

Влияет на скорость эволюции политики в процессе обучения. Оно соответствует порогу допустимого отклонения между старой и новой политикой при обновлении методом градиентного спуска.Установка меньшего значения приводит к более стабильным обновлениям, но также замедляет процесс обучения.

gamma (Изменяется в пределах 0.8 - 0.995)

Коэффициент дисконтирования для будущих вознаграждений от окружающей среды. Это можно представить как то, насколько далеко в будущем агент должен заботиться о возможном вознаграждении. Это значение должно быть большим в тех случаях, когда агенту необходимо предпринять действия сейчас, чтобы подготовиться к получению вознаграждения в отдаленном будущем. В случаях, когда награда более близка, это значение может быть не большим. Строго говоря, оно должно быть меньше 1.

lambd (Изменяется в пределах 0.9 - 0.95)

Параметр корректировки используемый для расчета обобщенной оценки преимуществ (GAE).Этот параметр можно представить как то, насколько сильно агент зависит от текущей оценкис тоимости при расчете обновленной оценки стоимости. Низкое значение соответствует тому, что агент больше полагается на текущую оценку стоимости (что может привести к большому смещению),в то время как высокое значение соответствует тому, что агент больше полагается навознаграждения,фактически полученные всреде (что может привести к большой дисперсии).Этот параметр обеспечивает баланс между этими двумя параметрами, и подходящие значения могут привести к более стабильному процессу обучения.

## Задание 3
### Задание 3 - Приведите примеры, для каких игровых задачи и ситуаций могут использоваться примеры 1 и 2 с ML-Agent’ом. В каких случаях проще использовать ML-агент, а не писать программную реализацию решения?

Использовать MLagent стоит когда нету прямого взаимодействия между игроком и каким-либо объектом который регулирует ИИ, например в играх по типу серии Civilisation, ибо ош

В ручную код стоит писать когда действия НПС которым управяет MLagent являются более сложными и многослойными, например в играх серий Fallout и Skyrim

## Выводы

Мы научились создавать связь между Google Sheets, Unity и JupiterNotebook. Основываясь на изученных данных смогли создать систему считывающую и генерирующую данные в разных источниках

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
