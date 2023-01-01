Vlákna se v jazyce Java vytváří dvěma způsoby:
- Odvozením od třídy `Thread`
- Implementací rozhraní `Runnable`

V obou případech se musí implementovat [[Metody|metoda]] se signaturou `public void run()`. Vlákno se ovšem spouští metodou `start()`.

```java
// Příklad vlákna odvozením od třídy Thread
class BasicThread extends Thread {
	public void run() { 
		//... 
	}
}

Thread thread = new BasicThread();
thread.start()
```

```java
// Příklad vlákna implementováním rozhraní Runnable
class BasicThread implements Runnable {
	public void run() { 
		//... 
	}
}

Runnable runnable = new BasicThread();

Thread thread = new Thread(runnable);
thread.start()
```