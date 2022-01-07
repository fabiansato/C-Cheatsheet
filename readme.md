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



### Extern
Para usarlos en diferentes lugares fuera de las funciones
```c
extern int a, b, c; 
```



### Constantes

```c
const int MONTH = 12;
const char CAR = '@';
const char STRING[] = "Programming in C" 
```

```c
 // Ejemplo de constantes literales enteras
123
1024L // entero long
4352U // entero unsigned
0xFF3A // hexadecimal

// Ejemplos de constantes literales reales
82.347
2.5E4
5.432E-3

// Ejemplos de constantes literales caracter

'A'
'b'
'c'

// Ejemplos de constantes literales de cadena

"Esta es una cadena"
```
constantes definidas:
```c
 #define PI 3.141516
#define MAX 48
```

constantes enumaradas:
```c
 enum Color favorit_color { Red, Orage, Yellow, Green, Blue, Purple}
```

------------------------

### String literals

En c no hay strings propiamente dicho, son arrays con chars dato por dato.
```c
 char STRING[] = "Programming in C" 
```


------------------------

### Define (preprocesor)

Una directiva de preprocesador es una instrucción que recibe el compilador y le indica que hay ciertas acciones a realizar antes de iniciar a compilar el programa. Se insertan al principio de cada programa, y se identifican por estar precedidas por el caracter # 

```c
#include <stdio.h>
```


---------------------
### Imprimir acentos
```c
printf("%c Ponemos el acento o tilde en canel%cn\n",162, 162); //ó
```
Es decir, invocar el código de carácter que corresponde a la letra acentuada...

Códigos:
```c
á: 160
é: 130
í: 161
ó: 162
ú: 163
Á: 181
É: 144
Í: 214
Ó: 224
Ú: 23
ñ: 164
Ñ: 165
```
