# Алгоритмы СУБД

В этом репозитории собраны алгоритмы и структуры данных, используемые в различных СУБД.

## Компоненты

СУБД - это комплексное ПО, поэтому для простоты следует выделить несколько компонентов в рамках, которых применимы те или иные алгоритмы.

Основными компонентами СУБД можно выделить:

- [Планировщик](./planner.md)
  - Алгоритмы соединения таблиц (DPsize,DPhyp...)
  - Оптимизации
- Движок выполнения
  - Алгоритмы во внешней памяти (сортировка)
  - Алгоритм вытеснения страниц
  - Алгоритмы работы узлов плана (хэширование, merge-sort)
- [Конкурентность](./concurrency-control.md)
  - 2PL
  - MVCC (разные варианты)
  - Гранулярные блокировки (БД/таблица/кортежы/диапазоны)
    - Orthogonal key value locking
- [Движок хранения](./storage.md)
  - Btree и другие индексы
  - Отказоустойчивость (WAL/UNDO)
  - Slotted-array
  - ARIES
- Кластер
  - Consistent hashing
  - Raft
  - Paxos

Что еще:

- Wide merging
- Orthogonal key value locking
- Foster Btree

Почитать:

- Hyungsoo Jung, Hyuck Han, Alan David Fekete, Gernot Heiser, Heon Young Yeom: A scalable lock manager for multicores. ACM SIGMOD 2013: 73-84.
- [JPS 10] Ryan Johnson, Ippokratis Pandis, Radu Stoica, Manos Athanassoulis, Anastasia Ailamaki: Aether: a scalable approach to logging. PVLDB 3(1): 681-692 (2010).



