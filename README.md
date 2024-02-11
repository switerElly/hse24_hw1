# hse24_hw1
### Варфоломеева Анастасия Андреевна БПМ213

[Ссылка на гугл коллаб](https://colab.research.google.com/drive/1zgT2NSYKPUHdJjcnC9Jsn9XZNC2OfDeD?usp=sharing)

## Анализ QC прочтений
Данные отчета FasQC приведены для файла SRR5836473_1. На следующих графиках можно заметить некоторые зависимости:

Наблюдается резкое падение качества чтений ближе к концу.
![Image alt](https://github.com/switerElly/hse24_hw1/blob/main/data/Screenshot%20from%202024-02-10%2023-14-04.png)

Большоое количество T~ 38% и малое содержание C ~12%. В теории значения должны быть в районе 25%.
![Image alt](https://github.com/switerElly/hse24_hw1/blob/main/data/Screenshot%20from%202024-02-10%2023-14-36.png)

Распределение сильно отличается от теоретического, есть 2 пика.
![Image alt](https://github.com/switerElly/hse24_hw1/blob/main/data/Screenshot%20from%202024-02-10%2023-14-48.png)

## Число ридов
BS-Seq | 11347700-11367700 | 40185800-40195800 | deduplication 
--- | --- | --- | ---
SRR5836473 | 551  | 194 | 81.72%
SRR3824222 | 1344 | 565 | 97.09%
SRR5836475 | 797  | 274 | 90.93%

## Рисунки с уровнем метилирования и покрытием

#### SRR5836473 - 8 Cell
| Read 1  | Read 2 |
| --- | --- |
| ![](https://github.com/switerElly/hse24_hw1/blob/main/data/Screenshot%20from%202024-02-11%2020-05-09.png)  | ![](https://github.com/switerElly/hse24_hw1/blob/main/data/Screenshot%20from%202024-02-11%2020-05-18.png)  |
#### SRR5836475 - ICM
| Read 1  | Read 2 |
| --- | --- |
| ![](https://github.com/switerElly/hse24_hw1/blob/main/data/Screenshot%20from%202024-02-11%2020-06-27.png)  | ![](https://github.com/switerElly/hse24_hw1/blob/main/data/Screenshot%20from%202024-02-11%2020-06-34.png)  |
#### SRR3824222 - Epiblast
| Read 1  | Read 2 |
| --- | --- |
| ![](https://github.com/switerElly/hse24_hw1/blob/main/data/Screenshot%20from%202024-02-11%2020-03-25.png)  | ![](https://github.com/switerElly/hse24_hw1/blob/main/data/Screenshot%20from%202024-02-11%2020-03-40.png)  |

На графиках можно заметить, что уровень метилирования на довольно высоком уровне у образца 8 cell (CpG колеблется в районе 43-44%), сильно хуже ICM (CpG 22-23%) и самый высокий у образца Epiblast (CpG 78-79%). Все соотносится с информацией, предоставленной в приложенной к заданию статье. Также для наших парных чтений наблюдаются заметные колебания - небольшой bias во втором риде. Но также полученные цифры немного отличаются от ожидаемых с статье: на ранних стадиях CpG метилирование уменьшается до некоторого минимума (около 25%), а затем по мере дифференцировки тканей, оно сильно увеличивается (около 90%) и остается таким на протяжении всей жизни организма.

## Гистограмы распределения метелирования цитозинов по хромосоме
![Image alt](https://github.com/switerElly/hse24_hw1/blob/main/data/Screenshot%20from%202024-02-11%2020-14-25.png)
![Image alt](https://github.com/switerElly/hse24_hw1/blob/main/data/Screenshot%20from%202024-02-11%2020-14-35.png)
![Image alt](https://github.com/switerElly/hse24_hw1/blob/main/data/Screenshot%20from%202024-02-11%2020-14-42.png)

Из графиков видно, что есть сходство с картинкой из статьи: сначала наблюдаем спад, подъем, спад и еще один подъем, если поочереди расставим гистограммы. Происходит то же самое, что и ожидалось, основываясь на данных из статьи.

## Уровень метилирования и покрытия

Метилирование
![Image alt](https://github.com/switerElly/hse24_hw1/blob/main/data/image_meth.png)

Покрытие
![Image alt](https://github.com/switerElly/hse24_hw1/blob/main/data/image_cov.png)

Видим, что здесь тоже соблюдается пропорция метилирования: Epiblast больше 8 Cell, а последний в свою очередь больше ICM. Это совпадает и с полученными выше данными, и с данными статьи.
