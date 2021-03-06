---
layout: post
title: Логотип Beats Audio в SVG
why: Показать простой пример рисования логотипа с использованием SVG
excerpt: Активное развитие мобильных устройств, на которых разрешение экрана уже больше, чем нам моем ноутбуке, заставляет задуматься
keywords: логотип beats audio, рисуем с svg, технология SVG
tags:
- SVG
---

Активное развитие мобильных устройств с разрешением экрана большим,
чем нам моем ноутбуке, заставляет задуматься. На ретина дисплеях <span class="file">.png</span> иконки теряют свое качество.
Аналогично происходит и с логотипами.
Решение проблемы заключается в использовании векторной графики вместо растровой.

В рамках этого поста хочу показать очень простой пример рисования логотипа с использованием технологии SVG.
В качестве примера я взял логотип компании **Beats Audio**, производящей наушники с высоким качеством звучания.

Логотип состоит из двух кругов красного цвета, белого четырехугольника и белого круга.

Для начала определим холст и его размеры:

{% highlight html %}
<svg width="700" height="600">
    <!-- Тут будет фигура-->
</svg>
{% endhighlight %}

К элементу <span class="file">svg</span> можно задавать и другие атрибуты: id, class и прочее. Но сейчас нам это не нужно, поэтому обойдемся заданием размеров холста.

Определимся с координатами. Все круги рисуем в центре холста, который находится в точке (350,300). Их радиусы равны 290, 150 и 90px. Фигуры будем рисовать, используя элемент <span class="file">&lt;circle&gt;</span>.

Осталось задать четырехугольник. Воспользуемся элементом  <span class="file">&lt;polygon&gt;</span>.  Атрибут **points** содержит серию пар х- и у-координат, разделенных пробелами.

{% highlight html %}
<svg width="700" height="600">
    <circle cx="350" cy="300" r="290" />
    <circle cx="350" cy="300" r="150" />
    <circle cx="350" cy="300" r="90" />
    <polygon points="200,300 270,180 270,0 200,0" />
</svg>
{% endhighlight %}

Вы можете заметить, что на данный момент у нас большая черная окружность с каким-то непонятным аппендиксом. Пришло время задать стили.

Для заливки фигур воспользуемся атрибутом **fill**. В логотипе присутствует два цвета:
<span class="file" style="color: #ed1c24;">&#35;ed1c24</span> и белый.

{% highlight html %}
<svg width="700" height="600">
    <circle cx="350" cy="300" r="290" fill="#ed1c24"/>
    <circle cx="350" cy="300" r="150" fill="#FFF"/>
    <circle cx="350" cy="300" r="90" fill="#ed1c24"/>
    <polygon points="200,300 270,180 270,0 200,0" fill="#FFF"/>
</svg>
{% endhighlight %}

Получим следующий результат:


<svg width="700" height="600">
    <circle cx="350" cy="300" r="290" fill="#ed1c24" stroke-width="0"/>
    <circle cx="350" cy="300" r="150" fill="#FFF" stroke-width="0"/>
    <circle cx="350" cy="300" r="90" fill="#ed1c24" stroke-width="0"/>
    <polygon points="200,300 270,180 270,0 200,0" fill="#FFF" stroke-width="0"/>
</svg>

### Вывод

Мы рассмотрели простой пример рисования логотипа с использованием технологии SVG при помощи элементов **circle** и **polygon**. Обратите внимание, что нам понадобилось всего 6 строк кода, чтобы нарисовать логотип.
