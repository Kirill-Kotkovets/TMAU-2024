# Лабораторная работа №2

## Задание

На C++ реализовать программу, моделирующую ПИД-регулятор, в качестве объекта управления используя математическую модель, полученную в предыдущей лабораторной работе. Использовать ООП, в программе должно быть не менее 3-х классов (+наследование).

## Ввод консоли

```cmd
        Linear parameters:
Enter a: 0.54
Enter b: 0.64
        Nonlinear parameters:
Enter a: 0.24
Enter b: 0.87
Enter c: 0.94
Enter d: 0.4
```

## Вывод консоли

```cmd
       Linear Model:
E = 5,                  Yt = 2.452,     Uk = 1.3
E = 5.548,              Yt = 3.63119,   Uk = 3.14248
E = 4.36881,            Yt = 5.15422,   Uk = 5.52221
E = 2.84578,            Yt = 6.41955,   Uk = 7.4993
E = 1.58045,            Yt = 7.27561,   Uk = 8.83689
E = 0.724391,           Yt = 7.76848,   Uk = 9.60699
E = 0.231525,           Yt = 8.00593,   Uk = 9.97801
E = -0.00592762,        Yt = 8.09097,   Uk = 10.1109
E = -0.0909729,         Yt = 8.09924,   Uk = 10.1238
E = -0.0992397,         Yt = 8.07746,   Uk = 10.0898
E = -0.0774614,         Yt = 8.05018,   Uk = 10.0471
E = -0.0501751,         Yt = 8.0277,    Uk = 10.012
E = -0.0276978,         Yt = 8.01259,   Uk = 9.98842
E = -0.0125879,         Yt = 8.00394,   Uk = 9.9749
E = -0.0039372,         Yt = 7.9998,    Uk = 9.96844
E = 0.000198706,        Yt = 7.99834,   Uk = 9.96616
E = 0.00165623,         Yt = 7.99823,   Uk = 9.96598
E = 0.00177362,         Yt = 7.99863,   Uk = 9.9666
E = 0.00137335,         Yt = 7.99912,   Uk = 9.96737
E = 0.000884415,        Yt = 7.99951,   Uk = 9.96799
E = 0.000485314,        Yt = 7.99978,   Uk = 9.96841
E = 0.000218645,        Yt = 7.99993,   Uk = 9.96865
E = 6.68502e-05,        Yt = 8.00001,   Uk = 9.96876
E = -5.16443e-06,       Yt = 8.00003,   Uk = 9.9688
E = -3.0117e-05,        Yt = 8.00003,   Uk = 9.9688
E = -3.16866e-05,       Yt = 8.00002,   Uk = 9.96879
E = -2.43431e-05,       Yt = 8.00002,   Uk = 9.96877
E = -1.55861e-05,       Yt = 8.00001,   Uk = 9.96876
E = -8.50149e-06,       Yt = 8,         Uk = 9.96876
E = -3.7961e-06,        Yt = 8,         Uk = 9.96875

        Nonlinear Model:
E = 5,                  Yt = 1.942,     Uk = 1.3
E = 6.058,              Yt = -3.646,    Uk = 3.27508
E = 11.646,             Yt = -0.0308169,Uk = 7.58768
E = 8.03082,            Yt = 4.15795,   Uk = 11.5767
E = 3.84205,            Yt = 6.73218,   Uk = 15.0814
E = 1.26782,            Yt = 9.10768,   Uk = 17.0033
E = -1.10768,           Yt = 8.89068,   Uk = 17.4315
E = -0.890681,          Yt = 8.76996,   Uk = 17.3142
E = -0.769962,          Yt = 8.3438,    Uk = 16.8655
E = -0.343803,          Yt = 8.10134,   Uk = 16.572
E = -0.101344,          Yt = 7.99706,   Uk = 16.3949
E = 0.00294182,         Yt = 7.98895,   Uk = 16.3326
E = 0.0110481,          Yt = 7.99639,   Uk = 16.3195
E = 0.00360519,         Yt = 8.00282,   Uk = 16.3218
E = -0.00282208,        Yt = 8.00332,   Uk = 16.3231
E = -0.00331508,        Yt = 8.0024,    Uk = 16.3226
E = -0.00240269,        Yt = 8.00131,   Uk = 16.3212
E = -0.00130865,        Yt = 8.00075,   Uk = 16.3202
E = -0.000748132,       Yt = 8.00045,   Uk = 16.3195
E = -0.000453318,       Yt = 8.00031,   Uk = 16.3191
E = -0.000313288,       Yt = 8.00022,   Uk = 16.3189
E = -0.000216907,       Yt = 8.00015,   Uk = 16.3187
E = -0.000149941,       Yt = 8.0001,    Uk = 16.3186
E = -0.000100323,       Yt = 8.00007,   Uk = 16.3185
E = -6.67938e-05,       Yt = 8.00004,   Uk = 16.3185
E = -4.42268e-05,       Yt = 8.00003,   Uk = 16.3185
E = -2.94906e-05,       Yt = 8.00002,   Uk = 16.3184
E = -1.96923e-05,       Yt = 8.00001,   Uk = 16.3184
E = -1.31854e-05,       Yt = 8.00001,   Uk = 16.3184
E = -8.81726e-06,       Yt = 8.00001,   Uk = 16.3184
```

![](../images/linearmodel.png)
![](../images/noninearmodel.png)

## Вывод

В ходе данной работы мы создали программу, моделирующую ПИД-регулятор, в качестве объекта управления используя математическую модель, полученную в предыдущей лабораторной работе.