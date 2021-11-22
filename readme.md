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


------------------------------
### Distintas versiones de GCC en Linux
Manipular distintas versiones de gcc
```linux
sudo apt install software-properties-common
sudo add-apt-repository ppa:ubuntu-toolchain-r/test
```
```linux
sudo apt install gcc-7 g++-7 gcc-8 g++-8 gcc-9 g++-9
```

```linux
sudo update-alternatives --install /usr/bin/gcc gcc /usr/bin/gcc-9 90 --slave /usr/bin/g++ g++ /usr/bin/g++-9 --slave /usr/bin/gcov gcov /usr/bin/gcov-9
sudo update-alternatives --install /usr/bin/gcc gcc /usr/bin/gcc-8 80 --slave /usr/bin/g++ g++ /usr/bin/g++-8 --slave /usr/bin/gcov gcov /usr/bin/gcov-8
sudo update-alternatives --install /usr/bin/gcc gcc /usr/bin/gcc-7 70 --slave /usr/bin/g++ g++ /usr/bin/g++-7 --slave /usr/bin/gcov gcov /usr/bin/gcov-7
```
```linux
sudo update-alternatives --config gcc
```


