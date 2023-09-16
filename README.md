# Reto Clase 3 😲
By Juan Esteban Molina Rey (eljuanessoy)
1. Algoritmo para obtener los números primos

Para el primer caso desarrolle el flujograma para determinar si un numero es o no es primo:
```mermaid
flowchart TB;
    A(INICIO)-- Ingresa un numero --> B[n]
    B --> C[X = 1]
    C --> D["c (Contador) = 0"]
    D --> E{X <= n}
    E -- NO --> J{C == 2}
    E -- SI --> F{n % X == 0}
    F -- SI --> H[c = c + 1]
    H --> I
    F -- NO --> I[X = X + 1]
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

si n mod x == 0 Entonces
c = c + 1
FinSi
Fin Para             
si c == 2 Entonces
Escribir «El numero «,n,» es primo»
SiNo
Escribir «El numero «,n,» no es primo»
FinSi     
FinAlgoritmo
```
