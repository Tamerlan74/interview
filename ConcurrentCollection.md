1. В чем необходимость Concurrent Collection?

- Традиционные коллекции не являются потокобезопасными. только несколько классов, таких как Vector, HashTable, являются потокобезопасными.
- Коллекции предоставляют некоторые методы, такие как synchronizedList, synchronizedMap, synchronizedSet, которые обеспечивают безопасность потоков, но проблема в том, что они захватывают блокировку при всей коллекции даже для чтения, которое снижает производительность.
- В традиционной коллекции, если один поток выполняет итерацию, а другой пытается изменить, возникает исключение ConcurrentModificationException.

2. Какие есть concurrent collection классы?

- ConcurrentHashMap
- CopyOnWriteArrayList
- CopyOnWriteArraySet

3. Почему производительность ConcurrentHashMap лучше чем HashTable и synchronizedMap?

В HashTable и synchronizedMap блокируется вся коллекция, поэтому только один поток может захватывать блокировку за раз, в то время как в ConcurrentHashMap блокировка получается на уровне сегмента, поэтому одновременно несколько потоков могут захватывать блокировку в разных разных сегментах.

4. Что такое уровень параллелизма в ConcurrentHashMap?

Уровень параллелизма определяет, сколько потоков может получить блокировку. По умолчанию ConcurrentHashMap имеет 16 сегментов, а уровень параллелизма также имеет 16 значений. Это означает, что 16 потоков могут принимать блокировку одновременно для каждого сегмента. Мы также можем изменить значение уровня параллелизма для Например, если мы сделаем 8, то все счетчики сегментов делятся на 8, и полученное количество сегментов будет сохранять единственную блокировку.

5. Что такое CopyOnWriteArrayList?

Это потокобезопасная версия List. Для каждой операции записи создается отдельная копия клона, и JVM синхронизирует клон и фактическую коллекцию.