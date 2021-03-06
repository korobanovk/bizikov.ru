---
layout: post
title: История вычисления числа Пи
keywords: Число Пи, История числа Пи
tags:
- Match
---

Сегодня мы прекрасно знаем о том, кто создал Фэйсбук, Вконтакте, кто создал первый компьютер, кто первый полетел в космос.
Но знаем ли мы того, кто первый догадался о связи длины окружности и ее диаметра?

Впервые обозначение \\(\pi \\) можно найти в работе "Synopsis Palmoriourum Matheseos" английского преподавателя Уильяма Джонса в 1706 году.

<blockquote>
&pi; - отношение длины окружности к длине ее диаметра;
</blockquote>

Обозначение \\(\pi \\) для числа 3,141592... получило большую популярность после того, как его стал применять выдающийся математик Леонард Эйлер в своих математических трудах.

<blockquote>
Нужно понимать, что обозначение ввели только в 1706 году, до этого число 3,141592.. не называли числом &pi;, но для удобства я буду называть его имеенно так.
</blockquote>

Вычисление числа \\(\pi \\) начинает свою историю с Древнего Вавилона. Как известно, жители Междуречья были отличными мастерами и инженерами, но в своих вычислениях они использовали довольно грубое прибличение \\(\pi \\).
Вавилоняне вели свои записи на глиняных табличках

![]({{ site.url }}/upload/article/2014/01/18/image_00.jpg)

<p class="image-description">Глинянная табличка из Вавилона. На ней изображено решение задачи для вписанной в квадрат окружности</p>

На современном языке вычисления древних вавилонян можно записать следующим образом:

\\[ S = \frac{C^{2}}{12} \\]

Где \\( S \\) - площадь круга, а \\( C \\) - длина ограничивающей его окружности. Способ применявшийся для вывода это формулы, неизвестен.

Если в нее подставить выражения площади круга \\( S = \pi r^{2} \\) и длины окружности \\( S = 2 \pi r^{2}\\), то получим:

\\[ \pi r^{2} = \frac{(2 \pi r)^{2}}{12} \\]

\\[ \pi r^{2} = \frac{4 \pi^{2} r^{2}}{12} \\]

\\[ \pi r^{2} = \frac{\pi^{2} r^{2}}{3} \\]

\\[ \pi = \frac{\pi^{2}}{3} \\]

\\[ \pi = 3 \\]

Более точное значение для \\(\pi \\) использовали древние египтяне. Наверное, многие слышали про папирус Ринда.

В Лондоне и Ною-Йорке хранятся две его части, назван папирус по имени мецената Генри Ринда, который купил его в 1858 году.

Папирус составил Армес, древнеегипетский писец, примерно между 2000-1700 годами до нашей эры.

Папирус содержит записи с решением различных практических задач.

На современном языке вычисления древних египтян можно записать как:

\\[ S = (d - \frac{1}{9d})^{2} = (1 - \frac{1}{9})^{2} d^{2}  \\]

Если мы воспользуемся уже известной нам формулой нахождения площади и выразим через нее \\(\pi \\), то получим выражения:

\\[\pi = \frac{S}{r^{2}} \\]

Возьмем \\(d = 1 \\), то \\(r = \frac{1}{2} \\)

\\[S = (1 - \frac{1}{9})^{2} d^{2} = (\frac{8}{9})^{2} = \frac{64}{81}\\]

Подставим получившийся результат в формулу

\\[\pi = \frac{S}{r^{2}} = \frac{\frac{64}{81}}{\frac{1}{4}} = \frac{64 \cdot 4}{81} = \frac{256}{81} = 3,16 \\]

Значительный прорыв в вычислении значения числа \\(\pi \\) произошел в Древней Греции.

Древние греки Евдокс, Гиппократ и многие другие - сводили измерение окружности к построению соответствующего отрезка, а измерение круга - к построению равновеликого квадрата.
Но не тут то было, они столкнулись с проблемой. Все их попытки сводились к выражению отношения длины окружности к диаметру (то есть числа \\(\pi \\)) рациональным число, и поэтому заранее были обречены на провал. Ведь как нам известно, иррациональное число нельзя представить на бумаге.

Со временем, математики поняли, что нужно искать новый подход к вычислению \\(\pi \\)
Математик, который впервые поставил задачу измерения круга на научную почву, был Архимед. Он получил свою оценку

\\[3\frac{10}{71} < \pi < 3\frac{1}{7}\\]

Архимед рассматривал отношение периметров вписанного и описанного 96-угольника к диаметру окружности, в результате чего получил приближенное значение

\\[\pi = 3,14\\]

Метод Архимеда довольно прост, но при отсутствии таблиц тригонометрических функций потребуется извлечение корней, а выполнение этой операции вручную отнимает много времени.
Один из минусов метода - это медленная сходимость. С каждой итерацией погрешность уменьшается лишь в 4 раза.

Даже с учетом такой сходимости, метод Архимеда был популярен аж до 17 века. До середины 17 века все попытки вычисления числа \\(\pi \\) европейскими математиками сводились к лишь к увеличению числу сторон многоугольника.

Около 265 года, китайский математик Лю Хуэй показал довольно простой и точный метод для вычисления \\(\pi \\). Он самостоятельно провел вычисление для 3072-угольника и получил приближенное значение следующим образом:

\\[ \pi =  A_{3072} = 3 \cdot 2^8 \cdot \sqrt{2-\sqrt{2+\sqrt{2+\sqrt{2+\sqrt{2+\sqrt{2+\sqrt{2+\sqrt{2+\sqrt{2+1}}}}}}}}} \approx 3,14159 \\]

Спустя пару веков, в 480 году еще китайский математик Цзу Чжунчжи используя метод Лю Хуэя вычислил приближенное значение числа \\(\pi \\) для 12288-угольник, получив следующий результат:

\\[\pi \approx \frac{355}{113} \approx 3,141592... \\]

Помимо этого, Цзу показал, что \\(3,1415926 < \pi < 3,1415927 \\).

Вычисленное им значение оставалось самым точным приближением числа \\(\pi \\)в течении следующих 900 лет.

В Древней Индии математик Арихабхата I в 5-6 веках умел вычислять число \\(\pi \\) с точностью до 4 знаков после запятой. В качестве приближения Арихабхата I использовал дробь:

\\[ \frac{62832}{20000} = 3,1416 \\]

В тексте "Ариабхатии" дробь определялась словестной формулировкой:

> Прибавьте 4 к 100, умножте на 8, прибавьте еще 62000, это будет для диаметра равного двум мириадам приближенная величина окружности

В 7 веке математик Брахмагупта дает грубое приближение числа \\(\pi \\):

\\[\pi = 3 \\]

А как более точное:

\\[ \pi = \sqrt{10} \\]

Методы, которые использователи Арихабхата и Брахмагупта, к сожалению нам не известны. Есть различне догадки, но я не буду о них рассказывать.

## Аналитический период


