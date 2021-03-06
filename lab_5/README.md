## Лабораторна робота № 5
## Тема: Визначення максимального потоку
## Мета роботи: Навчитись знаходити максимальний потік між парою вузлів та визначати мінімальний переріз.

**Хід роботи**

**1. За допомогою лабораторного макету побудувати випадковий неорієнтований зважений граф G={8,10}.**

![граф](https://github.com/Bohdansenyk/senyk-lab-totk-2021/blob/4ff97702a48f3fbfb75fad4e9a17b24e42749dc3/lab_5/lab5_1.png)

**2. Знайти шлях (вказати послідовність ребер) з максимальною пропускною здатністю (вказати якою) між вузлами i та j (i - вершина витоку (початкова); j - вершина стоку (кінцева)).**

Стік - Вершина 0.

Витік - Вершина 6.

0 -> 5 -> 6 = 10 

0 -> 1 -> 4 -> 5-> 6  = 1

0 -> 2 -> 6 = 4

**3. Визначити максимальний потік, який може бути переданий між вузлами i та j.**

Максимальний потік від вершини 0 до 6 = 10 + 1 + 4 = 15.

**4. Вказати ребра, які входять у мінімальний переріз (Переріз - видаляємо ребра графа так щоб не було шляхів між витоком і стоком).**

Ребра  0 -> 1, 0 -> 5  та 0 -> 2


**5.Визначити максимальний потік, який може виходити з вузла i. Визначити максимальний потік, який може входити у вузол j.**

максимальний потік, який може виходити з вузла 0 = 1 + 10 + 4 = 15

максимальний потік, який може входити у вузол 6 = 11 + 12 + 2 = 25

**6. Вважаючи, що між вузлами i та j передається максимальний потік, до яких вузлів можна здійснити передачу інформації з вузла і. Визначити пропускну здатність даних маршрутів.**

До жодних, бо   шляхи 0 -> 1, 0 -> 5 i 0 -> 2  не мають вільної пропускної здатності.

**7. Вважаючи, що між вузлами i та j передається максимальний потік, які вузли можуть здійснити передачу інформації до вузла j. Визначити пропускну здатність даних маршрутів.**

2 -> 3 -> 7 -> 6 = 2
7 -> 3 -> 2 -> 6 = 4

Висновок: на даній лабораторній роботі було знайдено шлях з максимальною пропускною здатністю (вказати якою) між вузлами i та j на неорієнтованому зваженому графі G={8,10}.
