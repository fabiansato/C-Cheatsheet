# Cheatsheet + Documentación Programación en C

------------------------------
## Instalación en Windows

```c

```

------------------------------
## Instalación en Linux
```c
sudo apt update
```
luego
```c
sudo apt install build-essential
```
```c
sudo apt-get install manpages-dev
```

```c
gcc --version
```

------------------------------
### Compilación en Linux
creación de archivo
```c
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


------------------------------
## Tipos de datos

```c
int
usigned int
short
unsinged short
long
unsinged long
float
double
long double

char
unsinged char
```

------------------------------
### Void
```c
viod funcion(){
}
```

------------------------------
### Enum
```c
enum weekDays {Sunday, Monday, Tuesday, Wednesday, Thursday, Friday, Saturday} 

```

------------------------------
### Llamada de variables
```c
%d Se utiliza para representar una parte de la memoria como un número entero. 

Placeholders usados en C 

%c - a character 

%s - a string 

%d - a decimal integer 

%o - an octal integer 

%x - a hexadecimal integer 

%p - an address (pointer) 

%f - for floats 

%e - a floating point number in scientific notation 

%E - a floating point number in scientific notation 

%% - The % symbol 
```



------------------------------
### Llamada de variables
```c

```



------------------------------
### Llamada de variables
```c

```



