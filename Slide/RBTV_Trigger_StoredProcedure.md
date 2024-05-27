# ON UPDATE RESTRICT ON DELETE CASCADE

## Cascade
![Cascade](https://nglthu.github.io/Database/img/cascade.png)

## Restrict

![Restrict](https://nglthu.github.io/Database/img/restrict.png)

## No Action


![No Action](https://nglthu.github.io/Database/img/noAction.png)

# Signal

```
SIGNAL is the way to “return” an error.
SIGNAL provides error information to a handler, to an outer portion of the application, or to the client.
It provides control over the error's characteristics (error number, SQLSTATE value, message).

Without SIGNAL, it is necessary to resort to workarounds such as deliberately referring to a nonexistent table to cause a routine to return an error.

```
https://dev.mysql.com/doc/refman/8.0/en/signal.html
# delimiter // delimter ;

+ mysql client program to define a stored program containing semicolon characters, a problem arises. By default, mysql itself recognizes the semicolon as a statement delimiter, so you must redefine the delimiter temporarily to cause mysql to pass the entire stored program definition to the server.

+ To redefine the mysql delimiter, use the delimiter command.
  ```
delimiter //
[code]

delimiter ;

  ```

to enable the entire definition to be passed to the server as a single statement, and then restored to ; before invoking the procedure.
This enables the ; delimiter used in the procedure body to be passed through to the server rather than being interpreted by mysql itself.

Example :

