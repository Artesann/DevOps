1. chdir("/tmp")
2. /usr/lib/locale/locale-archive
3. echo > /proc/<pid>/fd/<fd>
4. Процессы-зомби не занимают ресурсов, но занимают записи в таблице процессов, если записи закончатся, система не сможет создать процесс.
5. В файле trace.txt
6. uname. Part of the utsname information is also accessible via
       /proc/sys/kernel/{ostype, hostname, osrelease, version,
       domainname}.
7. Две команды через ; выполняются независимо друг от друга, если две команды записаны через &&, то вторая будет выполняться только при успешном завершении первой
8. -e  Exit immediately if a command exits with a non-zero status.  
   -u  Treat unset variables as an error when substituting.  
   -x  Print commands and their arguments as they are executed.  
   -o option-name pipefail - the return value of a pipeline is the status of
                           the last command to exit with a non-zero status,
                           or zero if no command exited with a non-zero status  
   Основная причина почему эту команду стоит использовать в скриптах автоматизации это возврат последнего не нулевого номера, с которым завершилась очередная команда из пайплайна
9. Больше всего процессов в статусе S - sleep