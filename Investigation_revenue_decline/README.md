# Анализ убытков приложения ProcrastinatePRO+

## Описание
Проведен анализ данных от ProcrastinatePRO+.
Рассчитаны различные метрики, использован когортный анализ: LTV, CAC, Retention rate, DAU, WAU, MAU и т.д. Использованы уже написанные ранее функции расчёта метрик. Сделаны правильные выводы по полученным данным.


## Инструменты
- Python
- Pandas
- Matplotlib
- когортный анализ
- юнит-экономика
- продуктовые метрики
- Seaborn

## Вывод:
  Как мы выяснили, реклама не окупается (низкий Roi). Связано это с ориентированием вложений компании в рекламные каналы с низким ROI (TipTop, FaceBoom), в один регион (US), вложения в который также не окупаются. Также мы видим, что только реклама на платформу PC окупается (хоть у него низкая конверсия, также и cac тоже низкий), хотя на данной платформе не так много пользователей нашего приложения.
Причина снижения окупаемости: 

1)TipTip (наш основной канал) не окупается вследствие постоянно растущей стоимости привлечения (CAC). Таким образом, с каждым месяцем расходы растут благодаря днамике данного канала.

2)FaceBoom и AdNonSense не окупаются из-за низкого LTV и превышающей LTV стоимости привлечения клиентов (CAC).

3)На рынке США вся реклама терпит убытки, вследствие того, что ни на одном устройстве реклама не окупается и стоимость привлечения (CAC) на всех устройствах быстро растет. TipTop и FaceBoom в США тоже не окупается по тем же причинам, что были перечислены выше.

4)В мировом масштабе реклама ни на одном устройстве не окупается из-за постонно растущей стоимости привлечения (CAC) всех устройств. Месяц назад PC еще окупался, однако на данный момент перестал.

5)Около 85% наших расходов на рекламу уходят на неокупающиеся каналы TipTop и FaceBoom, а на выгодные каналы привлечения (Yrabbit, MediaTornado, RocketSuperAds, lambdaMediaAds) комания средств почти не выделяет.

#### Рекомендации:
1)В большой степени пользоваться такими рекламными каналами, как Yrabbit, MediaTornado, RocketSuperAds, lambdaMediaAds, так как Roi у них больше 1, иногда и больше 2.

2)Снизить втрое затраты на TipTop и FaceBoom и перенаправить освободившиеся средства на вышеуказанные каналы

3)Активизировать рекламные компании в странах Европы (Германия, Великобритания, Франция). Снизить затраты на рекламные компании в США и перенаправить средства в вышеуказанные страны. Так как в США расходы на рекламу на всех устройствах растут и прекращение данного роста пока ожидать не приходится.

4)Соориентировать отдел маркетинга на оптимизацию рекламы на PC (может быть поправить интерфейс, сделать ее удобнее). Ну вообщем поработать над ней именно применимо к этому устройству. Также желательно провести данную работу касательно Android. Так как Android обладает наибольшим ROI в США (самый большой рынок нашей компании).
Благодаря выполнению этих пунктов, мы выйдим в плюс.
