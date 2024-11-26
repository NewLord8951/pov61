# pov61

Параграф 61.

1. Рекурсия — это определение, описание, изображение какого-либо объекта или процесса внутри самого этого объекта или процесса, то есть ситуация, когда объект является частью самого себя.

2. Рекурсивное определение состоит из двух частей: базового случая (условия, при котором рекурсия останавливается) и рекурсивного случая (где функция вызывает саму себя для решения подзадачи). Это необходимо для предотвращения бесконечной рекурсии и обеспечения завершенности.

3. Рекурсивная процедура или функция — это такая, которая вызывает саму себя в своем теле. Например, функция для вычисления чисел Фибоначчи: Фиб(n) = Фиб(n-1) + Фиб(n-2) при n > 1 Фиб(0) = 0, Фиб(1) = 1

4. Задача «Ханойские башни» состоит в том, чтобы переместить набор дисков с одного стержня на другой, используя третий стержень, при условии, что больше дисков нельзя помещать на меньшие. Рекурсивное решение заключается в перемещении n-1 дисков, а затем перемещении n-го диска.

5. Нерекурсивный алгоритм требует использования стека или очереди для отслеживания перемещений. Можно воспользоваться итеративным подходом и посчитать количество перемещений, а затем воспользоваться битовыми операциями для выяснения, какой диск стоит переместить на каждом этапе.

6. Процедуру Б можно назвать рекурсивной, если она вызывает саму себя. Процедура А может быть взаиморекурсивной, если она вызывает процедуру Б, а та уже вызывает А.

7.  Докажите, что в рассмотренных в параграфе задачах этого не случится. Рекурсия никогда не остановится, если отсутствует базовый случай или условие, при котором рекурсия завершается. Например, если функция всегда вызывает себя с одинаковыми параметрами, это приведет к бесконечной рекурсии. В задачах, рассмотренных в параграфе, базовые случаи со строгими условиями (например, 0 для факториала) предотвратят бесконечность.

8.  Как он используется при выполнении программ? Стек — это структура данных, работающая по принципу LIFO (последний пришел — первый вышел). В программировании стек используется для хранения контекста выполнения функций, включая локальные переменные и адрес возврата, что позволяет осуществлять управление памятью и выполнять рекурсию.

9.  Переполнение стека может произойти, если функции вызывают друг друга слишком много раз без достижения базового случая. Это приводит к тому, что стек затаскивает все больше и больше уровней вызова, что в конечном итоге приводит к недостатку памяти.

10. Назовите достоинства и недостатки рекурсии. Когда её следует использовать, а когда нет? Достоинства:

Упрощение кода и логики задач, особенно для структур, таких как деревья и графы.
Чистота и ясность алгоритмов.
Недостатки:

Возможное переполнение стека.
Более высокие затраты на память и вычислительные ресурсы.
Иногда может быть сложнее проанализировать производительность.
Рекурсию следует использовать при решении задач, которые естественно разбиваются на подзадачи (например, сортировка, обход деревьев). Не стоит использовать рекурсию, если известно, что глубина рекурсии может быть значительной или когда производительность критична.
