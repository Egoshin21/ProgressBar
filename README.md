<h1 align="center"> ProgressBar</h1>

# Содержание

1.[ProgressBar](https://github.com/Egoshin21/ProgressBar/blob/main/README.md#progressbar)

2.[ProgressBar (Horizontal)](https://github.com/Egoshin21/ProgressBar/blob/main/README.md#progressbar-horizontal)

3.[Indeterminate ProgressBar](https://github.com/Egoshin21/ProgressBar/blob/main/README.md#indeterminate-progressbar)

## Основы
Компонент ProgressBar (Индикатор прогресса) применяется в тех случаях, когда пользователю нужно показать, что программа не зависла, а выполняет продолжительную работу.

Находится в категории **Widgets.**

![asdfd](https://user-images.githubusercontent.com/78643217/145469276-958f5e43-e579-47d3-beaf-dee863b62b26.jpg)

Студия предлагает несколько видов индикаторов: **ProgressBar** и **ProgressBar (Horizontal).** В свою очередь компонент имеет несколько модификаций и их отличия заложены в стилях, если посмотреть XML-описание компонентов. Стили постоянно меняются, поэтому проще выбрать атрибут style и посмотреть предлагаемые варианты из выпадающего списка на текущий момент.

Методы для работы с **ProgressBar:**

* setProgress() — устанавливает заданное значение индикатора прогресса;
* getProgress() — возвращает текущее значение индикатора прогресса;
* incrementProgressBy() — устанавливает величину дискретизации приращения значения индикатора;
* setMax() — устанавливает максимальное значение величины прогресса.

## ProgressBar

Круговые индикаторы **Normal, Small и Large**  можно просто разместить на экране, и они будут бесконечно выводить анимацию вращения без единой строчки кода.

Как правило, "бесконечный" индикатор выводят в нужный момент, а когда задача выполнена, то его скрывают. Видимость можно установить через XML и программно.

Добавляем ProgressBar в  activity_main.xml

<img src="https://user-images.githubusercontent.com/78643217/145473716-023f108b-73da-42c3-842d-675b1e872331.jpg" width="500" />


Далее реализуем его в MainActivity c помощью **setVisibility**

<img src="https://user-images.githubusercontent.com/78643217/145473870-9ce60c67-0c3c-4355-a6fd-9cb5ed34bd57.jpg" width="600" />


В итоге должен выглядеть так:


<img src="https://user-images.githubusercontent.com/78643217/145474063-9b32159e-afa9-49d0-89c9-cb35a3e1ef62.jpg" width="400" />

# ProgressBar (Horizontal) 

Компонент **ProgressBar (Horizontal)** (Индикатор прогресса) применяется в тех случаях, когда пользователю нужно показать, что программа не зависла, а выполняет продолжительную работу.

Горизонтальный индикатор обычно используют, чтобы показать индикатор в действии. При длительной операции пользователь видит, что полоска индикатора постоянно увеличивается.


Добавляем ProgressBar в activity_main.xml

<img src="https://user-images.githubusercontent.com/78643217/145475643-de9caf9c-7fe4-498d-99bf-469516b2884c.jpg" width="600" />


Далее реализуем его в MainActivity

<img src="https://user-images.githubusercontent.com/78643217/145475701-9bdc5316-e637-4527-94d9-a30fb05df275.jpg" width="600" />

В итоге должен выглядеть так:

<img src="https://user-images.githubusercontent.com/78643217/145475799-5c9b3e3a-af11-4b6f-a840-54556b608725.jpg" width="400" />

# Indeterminate ProgressBar

**ProgressBar** может использоваться как для определенного(**Determinate ProgressBar**), так и для неопределенного(**Indeterminate ProgressBar**) хода выполнения задачи.

* Indeterminate ProgressBar используется, когда вы не можете оценить или отследить ход выполнения задачи. По умолчанию ProgressBar находится в неопределенном режиме.
* Determinate ProgressBar используется, когда вы можете оценить или отследить ход выполнения задачи.

Ход выполнения панели прогресса можно задать с помощью свойство прогресса, как показано ниже :
```
progressBar.progress = 70
```

Значение, указанное для свойства, представляет собой процент. Если 70 назначено прогрессу, то 70% панели прогресса будет помечено прогрессом.


Добавляем ProgressBar в activity_main.xml

<img src="https://user-images.githubusercontent.com/78643217/145478536-b0c54fec-39b8-4dd3-90a7-b0515834c178.jpg" width="600" />

И еще 2 кнопки:

<img src="https://user-images.githubusercontent.com/78643217/145478661-6ccbd85b-0cfb-48f2-8bf1-b8f188fb73dd.jpg" width="600" />

Далее реализуем его в MainActivity

<img src="https://user-images.githubusercontent.com/78643217/145478860-369f07b9-e578-4c92-a1b2-46d5232a3c0c.png" width="600" />

В итоге должен выглядеть так:

<img src="https://user-images.githubusercontent.com/78643217/145479066-731f7a71-f4cc-4426-b961-c02c7be8b0ca.jpg" width="400" />








