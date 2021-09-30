1. Файл node-exporter.service в файле `/etc/default/node-exporter` указано `ARGS=--web.listen-address=0.0.0.0:9111`
2. Файл basic_metrics.txt
3. Файл netdata.png
4. В выводе команды нашел такую строчку `[    3.455610] systemd[1]: Detected virtualization oracle.` systemd-detect-virt detects execution in a virtualized environment.
5. Лимит на количество открытых дескрипторов файла. `fs.nr_open = 1048576` С помощью ulimit можно посмотреть мягкие и жесткие ограничения, мягкое ограничение на колличество открытых файлов 1024, но его можно поднять до жесткого 1048576
6. Файл namespace.png
7. Fork-бомба. cgroup ограничивает количество процессов для среза. Посмотреть текущие настройки можно `cat /sys/fs/cgroup/pids/user.slice/user-1000.slice/pids.max`, изменить `echo 10 | sudo tee /sys/fs/cgroup/pids/user.slice/user-1000.slice/pids.max` 