# Module 10 Reflection

### Add another print just after the spawn
![img_01](figs/img_01.png)
As we can see, the program prints "hey hey" (the text outside the spawner) first, followed by "hola hola!" and "halo halo!".
"hey hey" is printed first because it's part of the synchronous code that gets executed immediately when the function runs.
Meanwhile, "hola hola!" and "halo halo!" are inside the spawner as asynchronous tasks — they are queued and wait to run until `executor.run()` is called.