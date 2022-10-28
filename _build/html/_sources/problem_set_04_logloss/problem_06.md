# 6. Температура генерации

Иногда в функцию $\softmax$ добавляют дополнительный параметр $T$, который называют температурой. Тогда она приобретает вид 

$$ 
f(z) =  \frac{e^{\tfrac{z_i}{T}}}{ \sum_{k=1}^K e^{\tfrac{z_k}{T}}}
$$

Обычно это делается, когда с помощью нейросетки нужно сгенерировать какой-нибудь новый объект. Пусть у нас есть три класса. Наша нейросеть выдала на последнем слое числа $1,2,5$. 

__а)__ Какое итоговое распределение вероятностей мы получим, если $T = 10$? А если $T = 1$? А если $T = 0.1$? 

```{dropdown} Решение

```

__б)__ Какое распределение получится при $T \to 0$? А при $T \to \infty$? 

```{dropdown} Решение

```

__в)__ Предположим, что объектов на порядок больше. Например, это реплики, которые Алиса может сказать вам в ответ на какую-то фразу.  Понятное дело, что вашей фразе будет релевантно какое-то подмножество ответов. Какое значение температуры сэмплирования $T$ смогут сделать реплики Алисы непредсказуемыми? А какие сделают их однотипными? 

```{dropdown} Решение

```
