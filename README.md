#Visual VM

Запустив проект "JvmExperience" программа выполнилась за 50 секунд.

Размер кучи начинался с 368 Мб, используя при этом 11 Мб.

![](https://github.com/Gangsta-Nick/JVM-Experience/blob/main/Screenshots/HeapStart.png?raw=true)

После сборки мусора размер кучи уменьшился, и принял минимальные значения, которые составляли 40 Мб размер кучи и 10.22 Мб используемой.

![](https://github.com/Gangsta-Nick/JVM-Experience/blob/main/Screenshots/HeapMin.png?raw=true)

По мере работы программы куча резко увеличилась, сбор мусора больше не происходил. Размер кучи увеличился до 720 Мб, использовалось 427.6 Мб.

![](https://github.com/Gangsta-Nick/JVM-Experience/blob/main/Screenshots/HeapUp.png?raw=true)

Максимальное значение куча приобрела в самом конце компиляции составила 2120 Мб (2 Гб), и  использовавшийся 632. (Не знаю зачем был создан почти 4-х кратный резерв кучи)

![](https://github.com/Gangsta-Nick/JVM-Experience/blob/main/Screenshots/HeapMax.png?raw=true)

Значение Metaspace началось с минимальных значений. Резерв составлял 3.25 Мб, использовалось 3.12 Мб.

![](https://github.com/Gangsta-Nick/JVM-Experience/blob/main/Screenshots/MetaSpaceMin.png?raw=true)

после чего резерв увеличился до 9.43 Мб, использовал ~9.16 Мб

![](https://github.com/Gangsta-Nick/JVM-Experience/blob/main/Screenshots/MetaspaceFirstUp.png?raw=true)

Следующий скачёк Metaspace зарезервировал 21.19 Мб, используя из них 20.9 Мб.

![](https://github.com/Gangsta-Nick/JVM-Experience/blob/main/Screenshots/MetaspaceSecondUp.png?raw=true)

Максимальное же значение Metaspace достигло по итогу выполнения, резерв составлял ~24.93 Мб, потребляя ~24.66 Мб.

![](https://github.com/Gangsta-Nick/JVM-Experience/blob/main/Screenshots/MetaspaceMax.png?raw=true)

При запуске Classes значения составляли 1074 shared, 2481 total. 

![](https://github.com/Gangsta-Nick/JVM-Experience/blob/main/Screenshots/ClassesMin.png?raw=true)

При первом же скачке были зафиксированны загрузки 1085 shared (на 9 больше первоначальных значений), 3265 total загруженных классов.

![](https://github.com/Gangsta-Nick/JVM-Experience/blob/main/Screenshots/ClassesFirstUp.png?raw=true)

Следующая загрузка классов составила 1088 (на 3 больше 2-й загрузки) shared, и 5346 total.

![](https://github.com/Gangsta-Nick/JVM-Experience/blob/main/Screenshots/ClassesSecondUp.png?raw=true)

По итогу выполнения программы количество загруженных shared классов не изменилось, total вырос до 6239 (6240) классов.

![](https://user-images.githubusercontent.com/88729303/153416314-20902683-092e-4588-b2b0-2074e4d06343.png)
