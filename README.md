# field_development
# Описание проекта

* Отрасль: нефтедобыча


* Цель: определить наиболее выгодный регион разработки.
* Процесс выбора регионов для разработки:
    - В избранном регионе собирают характеристики для скважин: **качество нефти и объём её запасов**;
    - Строят **модель для предсказания объёма запасов** в новых скважинах;
    - Выбирают скважины с **самыми высокими оценками значений**;
    - Определяют регион с **максимальной суммарной прибылью** отобранных скважин.
 
 
* Данные предоставлены пробы нефти в трёх регионах. Характеристики для каждой скважины в регионе уже известны.
* Описание данных:
    - id — уникальный идентификатор скважины;
    - f0, f1, f2 — три признака месторождения (вероятно это характеристики качества нефти и параметры, характеризующие размер месторождения). Заказчик, возможно, не желает раскрывать суть данных характеристик, но говорит об их значимости при построении моделей;
    - product — объём запасов в скважине (тыс. баррелей).
  
  
* Задачи:
    - Построить модели (линейной регрессии) предсказания объемов запасов;
    - На основе предсказаний модели оценить прибыль с учетом заданных параметров
    - Оценить риски разработки каждого из регионов
    - Выбрать наиболее выгодный с точки зрения прибыльности регион разработки
    
    
* Дополнительные условия:
    - Для обучения модели подходит только линейная регрессия (остальные — недостаточно предсказуемые).
    - При разведке региона **исследуют 500 точек**, из которых с помощью машинного обучения **выбирают 200 лучших** для разработки.
    - **Бюджет на разработку** скважин в регионе — **10 млрд рублей**.
    - При нынешних ценах **один баррель сырья приносит 450 рублей дохода**. 
    - После оценки рисков **нужно оставить лишь те регионы, в которых вероятность убытков меньше 2.5%**. Среди них выбирают регион с наибольшей средней прибылью.
