# Reto Clase 3 😲
By Juan Esteban Molina Rey (eljuanessoy)
1. Algoritmo para obtener los números primos

Para el primer caso desarrolle el flujograma para determinar si un numero es o no es primo:
```mermaid
flowchart TB;
    A(INICIO)-- Ingresa un numero --> B[n]
    B --> C[x = 1]
    C --> D["c (Contador) = 0"]
    D --> E{x <= n}
    E -- NO --> J{C == 2}
    E -- SI --> F{n % x == 0}
    F -- SI --> H[c = c + 1]
    H --> I
    F -- NO --> I[x = x + 1]
    I --> E
    J -- SI --> K[/El numero n es primo/]
    J -- NO --> L[/El numero n no es primo/]
    K --> M
    L --> M(FIN)
```
Pseudocodigo:
```pseudocode
Algoritmo Numeros Primos
n seran numeros enteros
X = 1
(c es un contador)
Inicio
ingresar un numero (n)
leer n
c = 0
x = 1
si x <= n hacer
    si n % x == 0 entonces
        c = c + 1 , x = x + 1 y repetir proceso
    sino solamente x = x + 1 y repetir proceso
finsi
si x > n entonces     
    si c == 2 entonces
        El numero n es primo
    finsi    
    sino
        El numero n no es primo
    finno     
FIN
```

2. Algoritmo para obtener la raiz cuadrada de un numero

Para el segundo caso desarrolle el flujograma para calcular la riaz cuadrada de un numero:
```mermaid
flowchart TB;
    A(INICIO)-- Ingresa un numero --> B[n]
    B --> C{n >= 0}
    C -- NO --> E[/No se puede calcular/]
    C -- SI --> D[x = n ** 0.5]
    D --> F[/x es la raiz cuadrada de n/]
    E --> G(FIN)
    F --> G
```
Pseudocodigo:
```pseudocode
Algoritmo Raiz Cuadrada
n tomará el valor de cualquier numero real
x = resultado de raiz cuadrada de n
Inicio
ingresar un numero (n)
leer n
    si n >= 0 entonces
        x = n ** 0.5
            escribir "x es la raiz cuadrada de n"
    sino
        escribir "No se puede calcular"
    finsi
    finno
FIN
```
