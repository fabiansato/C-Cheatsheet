# Cheatsheet + Documentación Programación en C

```linux

```
------------------------------
## Instalación en Windows

------------------------------
## Instalación en Linux
```linux
sudo apt update
```
luego
```linux
sudo apt install build-essential
```
```linux
sudo apt-get install manpages-dev
```

```linux
gcc --version
```

------------------------------
### Compilación en Linux
creación de archivo
```linux
nano hello.c
```
ejemplo:
```c
#include <stdio.h>
int main()
{
  printf ("Hello World!\n");
  return 0;
}

```
compilar en linux
```linux
gcc hello.c -o hello
```

ejecutar en linux
```linux
./hello
```




