### Задача №2. Разная комиссия
В прошлый раз мы рассматривали упрощённый вариант вычисления комиссии. Давайте усложним задачу. Теперь сумма комиссии будет зависеть ещё и от типа карты, с которой мы переводим средства.

За переводы с карты Mastercard комиссия не взимается, пока не превышен месячный лимит в 75 000 руб. Если лимит превышен, комиссия составит 0,6% + 20 руб.
За переводы с карты Visa комиссия составит 0,75%, минимальная сумма комиссии 35 руб.
За переводы с карты Мир комиссия не взимается.
Кроме того, введём лимиты на суммы перевода за сутки и за месяц. Максимальная сумма перевода с одной карты:

150 000 руб. в сутки
600 000 руб. в месяц
Комиссия в лимитах не учитывается.

Т. е. если пользователь решит перевести матери 150 000 руб. с карты Mastercard впервые за месяц, то его мать получит всю сумму, а комиссия будет удержана сверх этого. Сумма комиссии составит 75 000 * 0,006 + 20 = 470 руб. (т. к. с первых 75 000 руб. комиссия не взимается).

Напишите алгоритм расчёта в виде функции, передавая в функцию:

тип карты (по умолчанию Мир);
сумму предыдущих переводов в этом месяце (по умолчанию 0 рублей);
сумму совершаемого перевода.
В случае превышения какого-либо из лимитов операция должна блокироваться.