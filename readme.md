# Что это?

Небольшой скрипт, который высчитывает интеграл двух функций по трем входным переменным:

- h -- так же известна как длина шага, так неазываемая "дельта x"
- a -- точка начала отрезка интегрирования
- b -- точка конца отрезка интегрирования

# Как работает?

Реализованы два метода, которые принимают указанные выше параметры на вход.

- Метод трапеций известен как замена функции на ломаную. Считается по формлуе h * (f(a) + f(b))/2 + f(i) для i (a, b)
- Метод Симпсона. Он же -- метод парабол. Считается по формуле ℎ/3  ∗ (𝑓(a) + 𝑓(b) + удвоенная сумма всех других четных индексов + учетверенная сумма всех значений от нечетных индексов.


# А будут примеры?

Да, будет один. В скрипте указаны входные данные h = 1, a = 0, b = 2, на выходе будет следующее:

```
Input is:
a =  0
b =  2
h =  1

Function f1
Trapezoid:  4.0
Simpson:  4.0
The correct is 4

Function f2
Trapezoid:  7.0
Simpson:  6.0
The correct is 6
```