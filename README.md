Метод ближайшего соседа

Рассмотрим задачу kNN при k = 1 на языке R.

Алгоритм
Для классификации каждого из объектов тестовой выборки необходимо последовательно выполнить следующие операции:

Вычислить расстояние до каждого из объектов обучающей выборки
Найти объект из тренировочной выборки, от которого расстояние до классифицируемого объекта будет минимальным
Класс классифицируемого объекта — это класс, ближайшего к нему объекта из обучающей выборки
Введём число точек в тестовой выборке (n). Теперь создадим n точек с ограничениями по длине и ширине лепестка при помощи cbind и runif. Отбразим тренировочную выборку. Рисуя тестовые точки, запускаем алгоритм 1NN для определения принадлежности одному из трёх существующих классов. В самой функции 1NN ищем ближайшего по Евклидову расстоянию соседа для текущей точки и возвращаем вид ириса для неё же. На рисунке ниже показан результат 10 случайно выбранных точек.

