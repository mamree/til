# Understanding top

First row:

```
top - 12:04:58 up 1 min,  1 user,  load average: 0.74, 0.29, 0.11
```

* current time (11:57:11)
* uptime of the machine
* how many users logged in
* load average (1/5/15 minutes)

References:

* http://blog.scoutapp.com/articles/2009/07/31/understanding-load-averages
* http://stackoverflow.com/questions/6481005/how-to-obtain-the-number-of-cpus-cores-in-linux-from-the-command-line


Second row:

```
Tasks: 124 total,   1 running, 123 sleeping,   0 stopped,   0 zombie
```

* Processes running in totals: 124
* Processes running: 1
* Processes sleeping: 123
* Processes temporarily put into the background and is no longer running (stopped): 0
* Processes waiting to be stopped from the parent process (zombie): 0

References:

* http://unix.stackexchange.com/a/116968/1026	
* https://www.howtogeek.com/119815/htg-explains-what-is-a-zombie-process-on-linux/
* https://zombieprocess.wordpress.com/what-is-a-zombie-process/
* http://stackoverflow.com/questions/3853845/in-nix-what-causes-sleeping-in-top-command
