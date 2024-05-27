# ON UPDATE RESTRICT ON DELETE CASCADE

## Cascade
![Cascade](https://nglthu.github.io/Database/img/cascade.png)

## Restrict

![Restrict](https://nglthu.github.io/Database/img/restrict.png)

## No Action


![No Action](https://nglthu.github.io/Database/img/noAction.png)

# Signal

```
SIGNAL is the way to “return” an error. SIGNAL provides error information to a handler, to an outer portion of the application, or to the client. Also, it provides control over the error's characteristics (error number, SQLSTATE value, message). Without SIGNAL, it is necessary to resort to workarounds such as deliberately referring to a nonexistent table to cause a routine to return an error. 
```
https://dev.mysql.com/doc/refman/8.0/en/signal.html
