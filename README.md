# Оцнка стоимости финансового интрумента
Анализ и прогнозирование временного ряда

## Описание финансового инструмента: 
Период действия: 01.10.2018-31.03.201
Продавец финансового инструмента обязуется ежедневно по требованию Покупателя поставлять 1 млн куб. м газа. Цена на поставляемый газ определяется Покупателем за день до поставки как минимум из котировки «на следующий день» + 2 евро и фиксированной цены, равной 260 евро/тыс. куб. м. При этом Покупатель имеет право продавать получаемый от Продавца 1 млн куб. м на хабе с поставкой «на следующий день» по соответствующей цене.
Исходные данные: временной ряд исторических котировок газа с поставкой на хаб ТТФ «на следующий день» за 01.01.2016-01.10.2018.

Задание 1.
Требуется оценить стоимость инструмента

Провел анализ инструмента. Выделил основные характеристики:

<img width="770" height="362" alt="image" src="https://github.com/user-attachments/assets/c0220511-d25a-4e6e-892c-7fd8b6c56537" />

Оценка проводилась методом Монте-Карло по формуле

<img width="1037" height="728" alt="image" src="https://github.com/user-attachments/assets/8f8a5028-54eb-4943-8b3d-1545a36d4063" />

Результат

<img width="976" height="215" alt="image" src="https://github.com/user-attachments/assets/f5a9e15a-4ddb-42cb-94d2-3074ffa6bc04" />

Расчет статистических показателей проводился в Excel

<img width="1705" height="650" alt="image" src="https://github.com/user-attachments/assets/36361a8f-0f40-4fd7-b60f-51fc0cc71480" />

Симуляция стоимости котировки также производилась в ксель

<img width="1702" height="448" alt="image" src="https://github.com/user-attachments/assets/17ed0377-910b-403d-9e17-70fedf1d4eac" />

И финальный расчет

<img width="1331" height="410" alt="image" src="https://github.com/user-attachments/assets/43f58199-db6b-45c0-ad6c-f134551508f3" />


Задание 2
В приложенном файле (data_EX2.csv) находятся исторические значения переменной Y и значения 6 переменных (X1 - X6), которые потенциально могут оказывать влияние на Y. Известно, что Y может зависеть от собственных исторических значений и некоторых переменных (X1-X6), а также их исторических значений.
Необходимо:
1.	Выделить значимые переменные (X1-X6), оказывающие влияние на Y. Оценить зависимость Y от значимых переменных (их предыдущих значений при необходимости), а также от собственных прошлых значений.
2.	Построить прогноз для пропущенных значений Y.

Оценка зависимости проводилась визуально после построения графика в Python

<img width="911" height="477" alt="image" src="https://github.com/user-attachments/assets/71b3f7dd-4dc2-4aa4-ae70-6499d981e206" />

<img width="946" height="492" alt="image" src="https://github.com/user-attachments/assets/b62a2604-8103-43e3-bf5a-d77d91c1be03" />

<img width="946" height="492" alt="image" src="https://github.com/user-attachments/assets/0f155f3f-bc17-44bc-a153-c085052055ec" />

Также была построена матрица корреляции для численной оценки зависимости

<img width="946" height="492" alt="image" src="https://github.com/user-attachments/assets/531fdf39-2ba9-4c9a-a2af-a810977f6044" />

Также была оценена зависимость значения временного ряда от собственного предыдущего значения

<img width="975" height="485" alt="image" src="https://github.com/user-attachments/assets/28263c7e-a686-4568-8768-f4a76e4297f1" />

И взаимосвязь факторов между собой

<img width="975" height="485" alt="image" src="https://github.com/user-attachments/assets/047ac5a5-10fe-49b3-bd15-f29630d3d440" />

Выделены факторы с наибольшей взаимозависимостью

<img width="885" height="333" alt="image" src="https://github.com/user-attachments/assets/772f0fa5-889a-4f19-8d61-5c421d99fa0c" />

Далее проведено обучение мдели

<img width="692" height="297" alt="image" src="https://github.com/user-attachments/assets/3dacd3f3-af2d-471a-bb2c-06046002d664" />

И восстановление значений ряда

<img width="686" height="511" alt="image" src="https://github.com/user-attachments/assets/187cffad-420f-4395-9700-0122cc9ba630" />

Задание 3
Требуется построить модель зависимости Y от X и прогноз на основе данных в файле

Была проведена визуальная оценка зависимости

<img width="756" height="462" alt="image" src="https://github.com/user-attachments/assets/76647cb2-da70-4942-8ed9-b8cdf62c2c60" />

<img width="865" height="426" alt="image" src="https://github.com/user-attachments/assets/050dfba9-fcc8-4624-8a1f-b56e7a26647e" />

В том задании прогноз делался в Excel

<img width="865" height="426" alt="image" src="https://github.com/user-attachments/assets/2e8ecc0c-3333-449a-b4c2-7dec577ae761" />

<img width="873" height="448" alt="image" src="https://github.com/user-attachments/assets/98d288a9-3f47-4ed7-90e4-ad167ae0d333" />
