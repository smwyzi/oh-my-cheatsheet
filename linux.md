##### 查看 core pattern 
```
cat /proc/sys/kernel/core_pattern
```

##### 设置 core 在当前目录
```
ulimit -c unlimited
sudo bash -c 'echo core.%e.%p > /proc/sys/kernel/core_pattern'
```