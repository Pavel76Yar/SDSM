# 6. Предотвращение перегрузок

В жизни любого маршрутизатора наступает момент, когда очередь переполняется. Куда положить пакет, если положить его решительно некуда — всё, буфер кончился, совсем, и не будет, даже если хорошо поискать, даже если доплатить.  
Тут есть два путя: отбросить либо этот пакет, либо те, что уже очередь забили.  
Если те, что уже в очереди, то считай, что пропалодё.   
А если этот, то считай, что и не приходил он.  
Эти два подхода называются [**Tail Drop** и **Head Drop**](tail-drop-i-head-drop.md) и выполняют функцию **AQM — Adaptive Queue Management** — то есть следят за заполнением очереди и предпринимают те или иные меры.

Другие механизмы AQM, которые подходят к вопросу более интеллектуально:

* [RED - Random Early Detection](red-random-early-detection.md)
* [WRED - Weighted Random Early Detection](wred-weighted-random-early-detection.md)
