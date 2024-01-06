# Reference:
HACKING THE ART OF EXPLOTATION - Jon Erickson

This program runs on Linux OS.
Since this is a multi-user program that writes to a file in the /var directory, it must be suid root.
Run the following commands in program's directory in order to compile & run in appropriate state:

```bash
$ gcc -o game_of_chance game_of_chance.c
$ sudo chown root:root./game_of_chance
$ sudo chmod u+s./game_of_chance
$./game_of_chance
