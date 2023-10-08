# Betriebsystem-Shell

This is an assignment as a requirement to take the exam for the operating system lecture (Betriebssystem). The resulting program is a Shell that can be run in the terminal on Linux. This assignment was programmed using C++.

This task is divided into 2 parts. The first part allows the Shell to run the basic commands available in the Shell such as cat, ls, echo, touch, and others. To be able to run these commands, I use the method of execvp() which is like the default terminal command on Linux. In addition, Shell at this first stage can run various types of commands, such as simple commands, redirections commands, and Pipelines.

In the second stage of Shell construction, Shell can improve the efficiency of data storage so that Shell can work faster. In this case, addresses from physical memory that are retrieved from virtual memory are put into the TLB (Translation Lookaside Buffer) table. TLB stores the transfer of address storage from virtual memory to physical memory. This caches logging is done based on the FIFO (First In First Out) principle. With these caches, retrieving data from frequently used memory will be faster. In addition, the second stage of Shell has another feature, where Shell can run Process in the background and foreground. The second stage Shell also has a status list, which records what processes are running, stopped, or finished with exit() or signal() status. Users can also stop the running process by using exit and signal.
