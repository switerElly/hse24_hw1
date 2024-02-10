# hse24_hw1
### Варфоломеева Анастасия Андреевна БПМ213

[Ссылка на гугл коллаб]([https://colab.research.google.com/drive/1adEVel6P7qKHvHKsaQzHZFRMijNlUubr?usp=sharing](https://colab.research.google.com/drive/1zgT2NSYKPUHdJjcnC9Jsn9XZNC2OfDeD?usp=sharing))

## Анализ QC прочтений
Данные отчета FasQC приведены для файла SRR5836473_1. На следующих графиках можно заметить некоторые зависимости:
Во-первых резкое падение качества чтений ближе к концу.
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
