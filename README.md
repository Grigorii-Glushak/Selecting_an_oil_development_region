# Выбор региона для разработки новых нефтяных месторождений
***Описание проекта:*** 

Допустим, вы работаете в добывающей компании «ГлавРосГосНефть». Нужно решить, где бурить новую скважину.

Вам предоставлены пробы нефти в трёх регионах: в каждом 10 000 месторождений, где измерили качество нефти и объём её запасов. Постройте модель машинного обучения, которая поможет определить регион, где добыча принесёт наибольшую прибыль. Проанализируйте возможную прибыль и риски техникой *Bootstrap.*

***План работы над проектом:***

1. Загрузка и подготовка данных;
2. Обучение и проверка модели;
3. Подготовка к расчёту прибыли;
4. Расчёт прибыли и рисков;
5. Общий вывод;

## Вывод
При подготовке данных для расчёта прибыли и рисков мы выявили, что для разработки одной скважины, необходимо вложить `50` миллионов рублей, а точка безубыточности будет в том случае, если в текущей скважине будет `не менее 111 единиц` продукта. Если сравнить со средним объёмом нефти по наши `3` регионам, то у каждого их них этот показатель меньше. Ближе всего первый и третий регион с `~93` единиыами продукта.


Затем мы написали формулу которая рассчитывает прибыль от полученного сырья. И проверив каждый участок на потенциальную бОльшую прибыль выявили, что самый большой доход из лучших `200` скважин можно получить если разрабатывать первый регион - `14 миллиардов`. Чистая прибыль `4 миллиарда`.

Ну и в конце исследования мы проверили наши регионы на ожидаемую среднюю прибыль из `200` скважин, которые выбирали из `500` случайных скважин региона. И так `1000` раз. Самая большая прибыль у второго региона `0.46 миллиарда`. И у него же самый низкий показатель риска - `1.5%`. Относительно конкурентных регионов у которых этот же показатель *значительно* больше `2.5%`, он самый подходящий для разработки. Можно его рекомендовать.
