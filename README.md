# Implementación del Algoritmo de Ordenamiento por Burbuja

## Descripción

Este proyecto consiste en la implementación del algoritmo de ordenamiento por Burbuja (*Bubble Sort*) utilizando el lenguaje de programación Java.

El objetivo es aplicar los conocimientos sobre algoritmos de ordenamiento interno mediante 
un programa que permita organizar un arreglo de números enteros de menor a mayor.

El algoritmo realiza comparaciones entre elementos adyacentes y, cuando encuentra dos elementos en un orden incorrecto, 
intercambia sus posiciones hasta conseguir que todo el arreglo se encuentre ordenado.

## Tecnologías utilizadas

- **Java:** lenguaje de programación utilizado para desarrollar el algoritmo.
- **JDK:** herramienta necesaria para compilar y ejecutar el programa.
- **GitHub:** plataforma utilizada para almacenar y compartir el código fuente.

## Estructura del proyecto

El proyecto está organizado de la siguiente manera:

```text
OrdenaminetoInterno/
│
├── Burbuja.java
│
└── Main.java
```

### Descripción del codigo

**Burbuja.java**

Contiene la implementación del algoritmo de ordenamiento por Burbuja mediante el método `ordenar(int[] arr)`.

También incluye el método `imprimirArreglo(int[] arr)`, encargado de mostrar los elementos del arreglo en consola.

**Main.java**

Contiene el método principal `main()`, donde se declara el arreglo original, se muestra su contenido, se ejecuta el algoritmo de ordenamiento y finalmente se imprime el arreglo ordenado.

## Requisitos previos

Para ejecutar el proyecto es necesario contar con:

- Java JDK instalado.
- Una terminal o consola de comandos.
- Git instalado para clonar el repositorio.

Se puede comprobar la instalación de Java mediante los siguientes comandos:

```bash
java -version
javac -version
```

## Instalación y ejecución

### 1. Clonar el repositorio

Abrir una terminal y ejecutar el siguiente comando, sustituyendo la dirección por la URL de este repositorio:

```bash
git clone https://github.com/USUARIO/REPOSITORIO.git
```

### 2. Entrar a la carpeta del proyecto

```bash
cd REPOSITORIO
```

### 3. Compilar el programa

Ejecutar los siguientes comandos desde la carpeta principal del repositorio:

```bash
mkdir out
javac -d out OrdenaminetoInterno/*.java
```

En Windows PowerShell también se pueden utilizar:

```powershell
New-Item -ItemType Directory -Force out
javac -d out .\OrdenaminetoInterno\*.java
```

### 4. Ejecutar el programa

Después de compilar correctamente los archivos, ejecutar:

```bash
java -cp out OrdenaminetoInterno.Main
```

## Ejecución

El programa utiliza el siguiente arreglo inicial:

```java
int[] arreglo = {6, 1, 5, 8, 3, 2, 7, 4};
```

La salida esperada en consola es:

```text
Arreglo original:
[6, 1, 5, 8, 3, 2, 7, 4]

Arreglo ordenado:
[1, 2, 3, 4, 5, 6, 7, 8]
```

## Funcionamiento del algoritmo

El algoritmo de Burbuja realiza las siguientes operaciones:

1. Recorre el arreglo mediante un ciclo externo.
2. Compara los elementos adyacentes mediante un ciclo interno.
3. Si el elemento actual es mayor que el siguiente, intercambia sus posiciones.
4. Utiliza una variable temporal para realizar el intercambio.
5. Comprueba si hubo intercambios durante cada pasada.
6. Si no se realizaron intercambios, termina anticipadamente porque el arreglo ya está ordenado.

## Complejidad del algoritmo

| Característica | Complejidad |
|---|---|
| Mejor caso | O(n) |
| Caso promedio | O(n²) |
| Peor caso | O(n²) |
| Espacio adicional | O(1) |

La optimización mediante la variable booleana `intercambiado` permite reducir el tiempo de ejecución cuando el arreglo ya se encuentra ordenado.

## Datos

Nombre: Camila amor del angel cervantes 

Maestro: Víctor Hugo Vásquez Herrera.


Este proyecto fue desarrollado con fines académicos como parte de las actividades de la asignatura Estructura de Datos.
