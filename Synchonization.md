# Concurrent vs Parallel vs Asynchronous

1. [Объясни concurrent?](#Объясни-concurrent?)
2. [Объясни parallel?](#Объясни-parallel?)
3. [Объясни asynchronous?](#Объясни-asynchronous?)

# Thread syncronization

1. [Что такое критический блок?](#Что-такое-критический-блок?)
2. [Что такое thread synchronization?](#Что-такое-thread-synchronization?)
3. [Объясните концепт happens before в синхронизации потоков](#Объясните-концепт-happens-before-в-синхронизации-потоков)

# Синхронизированный метод vs синхронизированный блок

1. [Как используется ключевое слово synchronized?](#Как-используется-ключевое-слово-synchronized?)
2. [В чем разница между синронизированным блоком и методом?](#В-чем-разница-между-синронизированным-блоком-и-методом?)
3. [Почему синхронизированный блок предпочтительнее синхронизированного метода?](#Почему-синхронизированный-блок-предпочтительнее-синхронизированного-метода?)

# Условная синхронизация

1. [Что такое условная синхронизация?](#Что-такое-условная-синхронизация?)

# Volotile

1. [Что такое volotile переменная?](#Что-такое-volotile-переменная?)

# static vs volotile

1. [Что такое static переменные?](#Что-такое-static-переменные?)
2. [почему изменение, внесенное одним объектом в статическую переменную, не отображается для объекта в другом потоке?](#почему-изменение,-внесенное-одним-объектом-в-статическую-переменную,-не-отображается-для-объекта-в-другом-потоке?)

# Thread local storage

1. [Что такое thread local storage?](#Что-такое-thread-local-storage?)
2. [Что следует хранить в локальном хранилище потоков?](#Что-следует-хранить-в-локальном-хранилище-потоков?)
3. [Почему бы вам не синхронизировать доступ к объектам, хранящимся в ThreadLocal Storage?](#Почему-бы-вам-не-синхронизировать-доступ-к-объектам,-хранящимся-в-ThreadLocal-Storage?)
4. [Почему вы должны удалять объект из локального хранилища потоков?](#Почему-вы-должны-удалять-объект-из-локального-хранилища-потоков?)

# wait() vs sleep()

1. [В чем разница между wait() и sleep()?](#В-чем-разница-между-wait()-и-sleep()?)

# joining threads

1. [Какова цель метода join()?](#Какова-цель-метода-join()?)

# atomic classes

1. [Что такое atomic classes?](#Что-такое-atomic-classes?)
2. [В чем разница между Atomic и Volotile?](#В-чем-разница-между-Atomic-и-Volotile?)

# Lock

1. [Объясните механизм блокировки в многопоточности?](#Объясните-механизм-блокировки-в-многопоточности?)

# SYNCHRONISERS

1. [Какова цель синхронизаторов?](#Какова-цель-синхронизаторов?)
2. [Какие типы синхронизаторов доступны в Java?](#Какие-типы-синхронизаторов-доступны-в-Java?)

# Barriers

1. [Объясни что такое Barrier synchronizer?](#Объясни-что-такое-Barrier-synchronizer?)
2. [Можно ли переиспользовать баррьер?](#Можно-ли-переиспользовать-баррьер?)
3. [Что, если один из потоков завершится,покаа другие потоки ждут в Барьере?](#Что,-если-один-из-потоков-завершится,-пока-другие-потоки-ждут-в-Барьере?)
4. [Для какой работы вы используете Barrier?](#Для-какой-работы-вы-используете-Barrier?)

# Semaphore

1. [Объясни что такое Semaphore?](#Объясни-что-такое-Semaphore?)
2. [Что произойдет, если вы вызовете release() больше раз, чем acquire()?](#Что-произойдет,-если-вы-вызовете-release()-больше-раз,-чем-acquire()?)
3. [Что-происходит,-когда-вы-вызываете-acquire(),-но-permits-отсутствуют?]
4. [Как получить взаимоисключающую блокировку с помощью семафора?](#Как-получить-взаимоисключающую-блокировку-спомощью-семафора?)
5. [Где используется семафор?](#Где-используется-семафор?)

# Phaser

1. [Объясни что такое Phaser?](#Объясни-что-такое-Phaser?)
2. [Можно ли переиспользовать Phaser?](#Можно-ли-переиспользовать-Phaser?)

# Latch

1. [Что такое latch?](#Что-такое-latch?)
2. [Как потоки узнают что надо выполняться?](#Как-потоки-узнают-что-надо-выполняться?)

# EXECUTOR FRAMEWORK

1. [Расскажи что такое Executor framework?](#Расскажи-что-такое-Executor-framework?)
2. [Каковы возможности фреймворка Executor?](#Каковы-возможности-фреймворка-Executor?)

# Executor Service

1. [Расскажи что такое Executor Service?](#Расскажи-что-такое-Executor-Service?)
2. [Как отслеживается прогресс и статус выполнения задач?](#Как-отслеживается-прогресс-и-статус-выполнения-задач?)
3. [Использует ли ExecutorService выделенные потоки для выполнения задач в очереди?](#Использует-ExecutorService-выделенные-потоки-для-выполнения-задач-в-очереди?)
4. [Как с ExecutorService получить результаты от нескольких задач?](#Как-с-ExecutorService-получить-результаты-от-нескольких-задач?)

# Fork-Join

1. [Объясните что такое Fork-Join?](#Объясните-что-такое-Fork-Join?)
2. [Как фреймворк Fork-Join помогает оптимизировать выполнение задач?](#Как-фреймворк-Fork-Join-помогает-оптимизировать-выполнение-задач?)

# Ответы на тему Fork-Join

1. ### Объясните что такое Fork-Join?

Фреймворк fork-join позволяет разбить определенную задачу на несколько воркеров, а затем дождаться результата, чтобы объединить их

[на верх](#Fork-Join?)

2. ### Как фреймворк Fork-Join помогает оптимизировать выполнение задач?

помогает вам использовать преимущества нескольких процессоров.

[на верх](#Fork-Join?)

# Ответы для Executor Service

1. ### Расскажи что такое Executor Service?

Java ExecutorService представляет собой механизм асинхронного выполнения, который может выполнять задачи одновременно. ExecutorService создает и поддерживает повторно используемый пул потоков для выполнения отправленных задач.

[на верх](#Executor-Service)

2. ### Как отслеживается прогресс и статус выполнения задач?

ExecutorService предоставляет объекты Future для отслеживания хода выполнения и статуса выполняемой задачи.

[на верх](#Executor-Service)

3. ### Использует ли ExecutorService выделенные потоки для выполнения задач в очереди?

Все задачи, переданные в Executor, ставятся в очередь, которые выполняются потоками пула потоков.

[на верх](#Executor-Service)

4. ### Как с ExecutorService получить результаты от нескольких задач?

CompletionService of Executor можно использовать для получения результатов из нескольких задач.

[на верх](#Executor-Service)

# Ответы для EXECUTOR FRAMEWORK

1. ### Расскажи что такое Executor framework?

Executor framework предоставляет инфраструктуру для выполнения набора связанных задач в потоках.

[на верх](#EXECUTOR-FRAMEWORK)

2. ### Каковы возможности фреймворка Executor?

- Создание и уничтожение потоков.
- Поддержание оптимального количества потоков для задачи.
- Параллельное и последовательное выполнение задач.
- Разделение подтверждение выполнения задачи и процесс выполнения задачи.
- Политики связаны с контролем выполнения задач.

[на верх](#EXECUTOR-FRAMEWORK)

# Ответы для Latch

1. ### Что такое latch?

Latch заставляет группу потоков ждать завершения набора операций.

[на верх](#Latch)

2. ### Как потоки узнают что надо выполняться?

Все потоки ждут вызова метода await() до тех пор, пока countDown() не будет вызван столько раз, сколько установлен счетчик защелок.

[на верх](#Latch)

# Exchanger

1. [Что такое Exchanger?](#Что-такое-Exchanger?)

# Ответы для Exchanger

1. ### Что такое Exchanger?

позволяет двум потокам ждать друг друга в точке синхронизации для обмена элементами.

[на верх](#Exchanger)

# Ответы для Phaser

1. ### Объясни что такое Phaser?

Phasre очень похож на Barrier, также потоки ждут друг друга в точке синхронизации и потом продолжат рабоатть дальше, но в отличии от Barrier количество потоков меняется динамически

[на верх](#Phaser)

2. ### Можно ли переиспользовать Phaser?

да, можно

[на верх](#Phaser)

# Ответы для Semaphore

1. ### Объясни что такое Semaphore?

Семафор поддерживает определенное количество разрешений на доступ к уязвимому коду.

[на верх](#Semaphore)

2. ### Что произойдет, если вы вызовете release() больше раз, чем acquire()?

Если release() вызывается больше раз, чем acquire(), то для каждого такого дополнительного release будет добавлено дополнительное permit.

[на верх](#Semaphore)

3. ### Что происходит, когда вы вызываете acquire(), но permits отсутствуют?

Каждый вызов метода acquire() блокируется до тех пор, пока разрешение не станет доступным.

[на верх](#Semaphore)

4. ### Как получить взаимоисключающую блокировку спомощью-семафора?

Если вы хотите получить взаимоисключающую блокировку, инициализируйте семафор только с одним permit

[на верх](#Semaphore)

5. ### Где используется семафор?

Семафор обычно используется для обеспечения ограниченного доступа к дорогостоящему ресурсу.

[на верх](#Semaphore)

# Ответы для Barriers

1. ### Объясни что такое Barrier synchronizer?

В барьерах набор потоков ожидает друг друга, в точке синхронизации, прежде чем двигаться вперед.

[на верх](#Barriers)

2. ### Можно ли переиспользовать баррьер?

да

[на верх](#Barriers)

3. ### Что, если один из потоков завершится,покаа другие потоки ждут в Барьере?

Если какой-либо из потоков преждевременно завершен, все остальные потоки, ожидающие в точке барьера, также будут завершены.

[на верх](#Barriers)

4. ### Для какой работы вы используете Barrier?

Барьеры обычно используются, когда вы разделяете операцию на несколько задач, выполняемых в разных потоках, и ждете завершения всех задач, прежде чем двигаться дальше.

[на верх](#Barriers)

# Ответы для SYNCHRONISERS

1. ### Какова цель синхронизаторов?

Синхронизаторы синхронизируют несколько потоков для защиты уязвимого участка кода.

[на верх](#SYNCHRONISERS)

2. ### Какие типы синхронизаторов доступны в Java?

Barrier
Semaphore
Phaser
Exchenger
Latch

[на верх](#SYNCHRONISERS)

# Ответы для Lock

1. ### Объясните механизм блокировки в многопоточности?

Блокировка - это механизм управления доступом к общим ресурсам в многопоточной системе. Блокировку можно получить и снять в разных критических блоках кода.

[на верх](#Lock)

# Ответы для atomic classes

1. ### Что такое atomic classes?

Атомарные классы предоставляют возможность выполнять атомарные операции с примитивными типами, так что только одному потоку разрешено изменять значение до завершения вызова метода.

[на верх](#atomic-classes)

2. ### В чем разница между Atomic и Volotile?

Атомарные переменные обеспечивают атомарный доступ даже для составных операций, таких как операции до и после инкремента, что невозможно, если переменная объявлена как Volatile. Volatile просто гарантирует, что happens before чтение.

[на верх](#atomic-classes)

# Ответы для joining threads

1. ### Какова цель метода join()?

Потоки обычно объединяются, когда между потоками существует зависимость.
Метод join() целевого потока используется для приостановки текущего потока.
В таких ситуациях текущий поток не может продолжаться, пока целевой поток, от которого он зависит, не завершит выполнение.

[на верх](#joining-threads)

# Ответы для wait() vs sleep()

1. ### В чем разница между wait() и sleep()?

wait() вызывается на мониторе объекта; тогда как sleep() вызывается в потоке.
Объекты ожидания могут быть уведомлены; тогда как спящий поток не может.
Спящий поток не может снять блокировку; тогда как ожидающий объект может.
Чтобы разбудить спящий поток, вам нужна ссылка на него, которая не нужна для ожидающего объекта.

[на верх](#wait()-vs-sleep())

# Ответы для Thread local storage

1. ### Что такое thread local storage?

это локальная память потока

[на верх](#Thread-local-storage)

2. ### Что следует хранить в локальном хранилище потоков?

Идентификаторы транзакции или пользователя, в общем текущие рабочие данные

[на верх](#Thread-local-storage)

3. ### Почему бы вам не синхронизировать доступ к объектам, хранящимся в ThreadLocal Storage?

потому что они видны только в одном потоке

[на верх](#Thread-local-storage)

4. ### Почему вы должны удалять объект из локального хранилища потоков?

Чтобы предотвратить утечку, рекомендуется удалить объект ThreadLocal с помощью метода remove ().

[на верх](#Thread-local-storage)

# Ответы для static vs volotile

1. ### Что такое static переменные?

Статические переменные используются в контексте объектов класса, где существует только одна копия статической переменной, независимо от того, сколько объектов класса создано.

[на верх](#static-vs-volotile)

2. ### почему изменение, внесенное одним объектом в статическую переменную, не отображается для объекта в другом потоке?

если несколько потоков обращаются к одной и той же переменной, каждый поток сделает копию этой переменной в своем кэше ЦП, и изменения, сделанные потоком, не будут видны другим потокам.

[на верх](#static-vs-volotile-vs-synchronized)

# Ответы для Volotile

1. ### Что такое volotile переменная?

Поле, помеченное как volotile, сохраняется и считывается непосредственно из основной памяти. Поскольку volotile поля хранятся в основной памяти, все потоки видят самую обновленную копию значения volotile поля, независимо от того, какой поток изменил его.

[на верх](#Volotile)

# Ответы на тему Условная синхронизация

1. Условная синхронизация достигается с помощью условной переменной вместе с методами wait () и notify () или notifyAll ().

[на верх](#Условная-синхронизация)

# Ответы для Синхронизированный метод vs синхронизированный блок

1. ### Как используется ключевое слово synchronized?

Ключевое слово synchronized используется для обозначения критической части кода. Блокируется доступ для остальных потоков если критическую часть кода выполняет другой поток

[на верх](#Синхронизированный-метод-vs-синхронизированный-блок)

2. ### В чем разница между синронизированным блоком и методом?

Синхронизированный метод блокирует весь метод, синхронизированный блок блокирует тольуо критическую часть кода

[на верх](#Синхронизированный-метод-vs-синхронизированный-блок)

3. ### Почему синхронизированный блок предпочтительнее синхронизированного метода?

Предпочитайте синхронизированный блок синхронизированному методу, поскольку блокировка блокируется только для локального объекта, а не для всего объекта класса.

[на верх](#Синхронизированный-метод-vs-синхронизированный-блок)

# Ответы для Thread syncronization

1. ### Что такое критический блок?

это участок кода, который при одновременном доступе более чем одним потоком может оказать нежелательное влияние на результат.

[на верх](#Thread-syncronization)

2. ### Что такое thread synchronization?

контролирует доступ к критическим участкам кода для предотвращения нежелательных эффектов в программе.

[на верх](#Thread-syncronization)

3. ### Объясните концепт happens before в синхронизации потоков

Синхронизация создает буфер памяти, известный как «произошло до», который гарантирует, что любой другой поток, который впоследствии получает те же локальные объекты, может получить доступ ко всем изменениям, внесенным потоком в локальные объекты в критических секциях.

[на верх](#Thread-syncronization)

# Ответы для Concurrent vs Parallel vs Asynchronous

1.  ### Объясни concurrent?

это одновременное выполнение нескольких задач;
либо на нескольких ядрах, либо с помощью потока с приоритетным разделением времени на процессоре.

[на верх](#Concurrent-vs-Parallel-vs-Asynchronous)

2. ### Объясни parallel?

Это выполнение одной задачи на разных ядрах

[на верх](#Concurrent-vs-Parallel-vs-Asynchronous)

3. ### Объясни asynchronous?

это независимое выполнение процесса, не дожидаясь возврата значения от промежуточных операций.

[на верх](#Concurrent-vs-Parallel-vs-Asynchronous)