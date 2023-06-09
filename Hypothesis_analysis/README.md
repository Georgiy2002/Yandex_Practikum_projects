# Проверка гипотез по увеличению выручки в интернет-магазине — оценка результатов A/B теста

## Описание
Проведена приоритизация гипотез по фреймворкам ICE и RICE. Затем провел анализ
результатов A/B-теста, построил графики кумулятивной выручки, среднего чека,
конверсии по группам, а затем посчитал статистическую значимость различий конверсий
и средних чеков по сырым и очищенным данным. На основании анализа мной было
принято решение о нецелесообразности дальнейшего проведения теста.

## Инструменты
- Python
- Pandas
- Matplotlib
- SciPy
- A/B-тестирование
- проверка статистических гипотез

## Вывод
Принимаем следуещее решение: Останавливаем A/B-тест, зафиксировав победу группы B в конверсии по следующим причинам:
1)График средних чеков засвидетельствовал попадание серьезных выбросов после 17 августа в группу B, благодаря чему кумулитивный средний чек группы B надолго превзошел средний чек группы A. Однако тест Манна-Уитни, который процесс ранжирования нейтрализует пагубное влияние выбросов, выдал уровень значимости, согласно которому нельзя с уверенностью говорить о серезных различиях между двумя группами чеков. Данный тест с очищенными данными лишь еще раз подтвердил выводы первого. По двум тестам мы имеем довольно однозначный уровень значимости - это еще один довод в пользу остановки теста. Нет статистически значимого различия по среднему чеку между группами ни по «сырым», ни по данным после фильтрации аномалий. Исходя из вышесказанного, делаем вывод об отсутствие различий между средними чеками двух групп, несмотря на график.

 2)Абсолютно другая история со средним числом заказов на одного посетителя. Тест Манна-Уитни с "сырыми" данными и с "очищщенными" выдает довольно низкий уровень значимости, исходя из чего мы отвергаем гипотезу о равенстве кол-ва заказов на одного посетителя между двумя группами. Такой вывод подтверждает график, который также однозначно свидетельствует о наличие серьезных различий при отстуствие каких-либо значимых флуктуаций. Однозначность результатов теста Манна-Уитни и графика также доказывает нам бесполезность продолжения A/B теста.

 Таким образом, группа B превосходит группу A в кол-ве заказов на одного пользователя, однако группы равны в среднем чеке. Можно уверенно говорить, что изменения на сайте интернет-магазина привели к положительным изменениям, исходя из чего рекомендую принять нововведения.
