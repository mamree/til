# Kill Zombie Process

Get the zombie process PID, e.g: 1234

```
ps aux | grep -w Z 
```

Get the parent's process PID

```
ps o ppid 1234
```

Kill it

```
kill -9 3456
```
