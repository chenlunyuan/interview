# interview

## 说一说JMM
总：JMM是一套规范，java实现cpu多线程执行指令集时数据从主存加载到工作内存和从工作内存写回主存之间如何确保线程间的共享资源的可见性、一致性、原子性的一套规范
分：
1、多线程出现的并发问题，多个线程访问一个共享数据a, a被一个线程被修改，别的线程可能会因为不知道数据被修改，而用着已加载到其自己工作内存的数据，从而导致数据不一致
2、如何解决这个问题？在java语言中，可以用volatile来修饰变量，解决其可见性、一致性，一致性主要是体现在不让指令重排。
3、volatile 不能
