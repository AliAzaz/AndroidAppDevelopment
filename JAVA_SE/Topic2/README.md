## Concept of Static variable and Threading

### Static variable: 

Static variable is a variable that exists in the entire running of program. Means single copy of static variable is created and shared among all the instances of the class, they are class level variables. 
Likewise how many instances of class you create but static variable can't re-initialize. For example look [`Class 1a`](https://github.com/AliAzaz/AndroidAppDevelopment/blob/master/JAVA_SE/Topic2/src/class1/Class1a.java).

### Threading:

Thread is smallest sequence of program instruction that can can be managed independently by operating system.
In short: Divide long task to short task i.e thread.
* Each thread can run in parallel
* The OS divides processing time not only among different applications, but also among each thread within an application

For example look [`Class 1b`](https://github.com/AliAzaz/AndroidAppDevelopment/blob/master/JAVA_SE/Topic2/src/class1/Class1b.java) and [`Class 1c`](https://github.com/AliAzaz/AndroidAppDevelopment/blob/master/JAVA_SE/Topic2/src/class1/Class1c.java) .

#### Commonly used methods of Thread class:

`public void run()`: is used to perform action for a thread.<br />
`public void start()`: starts the execution of the thread.JVM calls the run() method on the thread.<br />
`public void sleep(long miliseconds)`: Causes the currently executing thread to sleep (temporarily cease execution) for the specified number of milliseconds.<br />
`public void join()`: waits for a thread to die.<br />
`public void join(long miliseconds)`: waits for a thread to die for the specified miliseconds.<br />
`public int getPriority()`: returns the priority of the thread.<br />
`public int setPriority(int priority)`: changes the priority of the thread.<br />
`public String getName()`: returns the name of the thread.<br />
`public void setName(String name)`: changes the name of the thread.<br />
`public Thread currentThread()`: returns the reference of currently executing thread.<br />
`public int getId()`: returns the id of the thread.<br />
`public Thread.State getState()`: returns the state of the thread.<br />
`public boolean isAlive()`: tests if the thread is alive.<br />
`public void yield()`: causes the currently executing thread object to temporarily pause and allow other threads to execute.<br />
`public void suspend()`: is used to suspend the thread(depricated).<br />
`public void resume()`: is used to resume the suspended thread(depricated).<br />
`public void stop()`: is used to stop the thread(depricated).<br />
`public boolean isDaemon()`: tests if the thread is a daemon thread.<br />
`public void setDaemon(boolean b)`: marks the thread as daemon or user thread.<br />
`public void interrupt()`: interrupts the thread.<br />
`public boolean isInterrupted()`: tests if the thread has been interrupted.<br />
`public static boolean interrupted()`: tests if the current thread has been interrupted.<br />