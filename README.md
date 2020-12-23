# concurrency
Playing with .net threads, basics of concurrency and functional programming.

# concepts
 - Concurrency is a process of doing more than one thing at a time.
 - Multithreading is a form of concurrency that uses multiple threads of execution.
 - Parallel processing is a process of doing lots of work by dividing it among multiple threads that run concurrently.
Parallel processing is one type of multithreading, and multithreading is one type of concurrency.
Another type of concurrency that is important in modern apps is async programming.
 - Asynchronous programming is a form of concurrency that uses futures or callbacks to avoid unnecessary threads.
 A future (promise) is a type that represents some operation that will complete in the future. The modern 
 future types in .net are Task and Task<TResult>.
 Asynchronous programming is centered around the idea of an asynchronous operation: some operation that is started
 that will complete some time later. While the operation is in progress, it does not block the original thread; the
 thread tharts the operation is free to do other work. When operation completes it notifies its future (Task) to
 let the application know the operation is finished.

 The better abstraction which can be applied here is that threading is about workers when asynchrony is about task.
