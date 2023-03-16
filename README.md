# TALLER #1
Fauel Joel Triana Pinilla
Andrés Felipe Sánchez Martínez
Juan David García Mendoza

En este repositorio queda evidenciado el proceso de solución de los puntos del taller #1 y su respectivo extra como lo es los diagramas de flujo, los cuáles de acuerdo al último dígito de las cedulas son 2, 6 y 8.

##### 1. Realice el quiz Python Beginner Quiz (20 preguntas) y adjunte pantallazo con el resultado (mínimo 90% bien).

A continuación, se adjuntan los pantallazos de cada uno de los resultados del quiz hecho por los participantes:

[![image.png](https://i.postimg.cc/G3YymNjh/image.png)](https://postimg.cc/QV8t6fPR)
[![image.png](https://i.postimg.cc/76CwZF8H/image.png)](https://postimg.cc/WFPQ9f1C)
[![image.png](https://i.postimg.cc/zXkZ8zbw/image.png)](https://postimg.cc/JGtdQWQt)

##### 2. Realice un programa que lea tres números reales y determine cuál es el mayor.

Para hallar la solucion al problema dos primero definimos las variables, ya creadas le pedimos al usuario que le de valor a esas variables y comenzamos a comparar la variable (a) con las demas para saber si esta es la mayor, si no es comparamos la (b) con las demas y en caso de que no hacemos lo mismo con la (c), y si no nos de mayor ninguna de las tres es porque todas las variables tienen el mismo valor.

```python
a : float
b : float
c : float
a = float(input("Ingrese el primer número real: "))
b = float(input("Ingrese el segundo número real: "))
c = float(input("Ingrese el tercer número real: "))
if a>b>c or a>c>b:
    print("El número mayor de los reales ingresados es " +str(a))
elif b>a>c or b>c>a:
    print("El número mayor de los reales ingresados es " +str(b))
elif c>a>b or c>b>a:
    print("El número mayor de los reales ingresados es " +str(c))
elif b==a and a==c:
    print("Los números reales ingresados son iguales ")
```
##### 3. Realice un programa que lea un número enteros y determine si es par o impar.

```python
n = int(input("Ingrese un número entero: "))
if n % 2 == 0:
    print("El número entero ingresado es par")
else:
    print("El número entero ingresado es impar")
```

##### 4. Realice un programa que lea dos números reales y determine si el primero es múltiplo del segundo.
La del cuarto comenzamos definiendo las variables y le pedimos al usuario ingresarlas, luego dividimos la variable (a) entre (b) y si el residuo es cero podemos decir que (a) es múltiplo de (b) en caso de que el residuo sea diferente a 0 quiere decir que (a) no es múltiplo de (b) y si (a) es igual a (b) no hacemos división y avisamos que ambos numeros son iguales.

```python
a = float(input("Ingrese el primer número real: "))
b = float(input("Ingrese el segundo número real: "))
if a % b == 0:
    print("El número " +str(a)+ " es múltiplo de " +str(b))
else:
    print("El número " +str(a)+ " no es múltiplo de " +str(b))
if a == b:
   print("Los números reales ingresados son los mismo")
```

##### 5. Realice un programa que lea tres números reales y determine si la suma de los dos primeros es mayor, menor o igual que el tercer número.

La del quinto definimos a, b y c como las variables que vamos a usar y con propiedad de float, luego efectuamos la suma de (a) y (b) y la comparamos con c, si es mayor a (c) damos la respuesta de que es mayor a (c) si no comparamos esperando que la suma sea menor a (c) si no es asi verificamos que sean iguales y mandamos el resultado.

```python
a = float(input("Ingrese el primer número real: "))
b = float(input("Ingrese el segundo número real: "))
c = float(input("Ingrese el tercer número real: "))
if (a+b)>c:
    print("La suma de " +str(a)+ " y " +str(b)+ " es mayor que el número " +str(c))
elif (a+b)<c:
    print("La suma de " +str(a)+ " y " +str(b)+ " no es mayor que el número " +str(c))
elif (a+b)==c:
    print("La suma de " +str(a)+ " y " +str(b)+ " es igual al tercer número real ingresado")
```
##### 6. Escriba un programa que solicite al usuario una letra y determine si es una vocal o una consonante.
Para el sexto punto, se declaró una s como una cadena, se pidió al usuario que ingresara cualquier letra y si ésta es una vocal, la consola dirá que la letra es una vocal, si no se cumple la condición, este aclarará que la ingresada no es una vocal; por ende, es una consonante.

````python
s = input("Ingrese cualquier letra: ")
if s == "a" or s == "e" or s == "i" or s == "o" or s == "u":
    print("La letra " +str(s)+ " es una vocal")
else:
    print("La letra " +str(s)+ " es una consonante")
````

##### Escriba un programa que pida 5 números reales y calcule las siguientes operaciones:
- El promedio
- La mediana
- El promedio multiplicativo (multilplica todos y luego calcula la raíz de la cantidad de operandos)
- Ordenar los números de forma ascendente
- Ordenar los números de forma descendente
- La potencia del mayor número elevado al menor número
- La raíz cúbica del menor número

Se le pide al usuario que ingrese 5 números, los cuales serán ordenados de forma ascendente y descendente. Después de eso, el programa evaluara el promedio, el cual se hace sumando los 5 números y dividiéndolos en 5. Después se toma la mediana, que al ser una cantidad de números impar, se toma el numero intermedio después de haberlos ordenado. Para sacar el promedio multiplicativo, se toman de igual manera los 5 números, se multiplican y luego al producto se le saca su raíz quinta. Luego el programa toma al mayor de los números y lo eleva por el numero menor. Por último, se toma el numero menor y se le saca su raíz cubica.

```python
a = float(input("Ingrese el primer número: "))
b = float(input("Ingrese el segundo número: "))
c = float(input("Ingrese el tercer número: "))
d = float(input("Ingrese el cuarto número: "))
e = float(input("Ingrese el quinto número: "))
promedio=float
mediana=float
prom_mult=float
potencia=float
raiz:float
#condicionales para ordenar los numeros de manera ascendente
if a > b:
    a, b = b, a
if a > c:
    a, c = c, a
if a > d:
    a, d = d, a
if a > e:
    a, e = e, a
if b > c:
    b, c = c, b
if b > d:
    b, d = d, b
if b > e:
    b, e = e, b
if c > d:
    c, d = d, c
if c > e:
    c, e = e, c
if d > e:
    d, e = e, d
print("Los números ordenados de forma ascendente son: ", a, b, c, d, e)
#condicionales para ordenar los numeros de manera descendente
if a < b:
    a, b = b, a
if a < c:
    a, c = c, a
if a < d:
    a, d = d, a
if a < e:
    a, e = e, a
if b < c:
    b, c = c, b
if b < d:
    b, d = d, b
if b < e:
    b, e = e, b
if c < d:
    c, d = d, c
if c < e:
    c, e = e, c
if d < e:
    d, e = e, d
print("Los números ordenados de forma descendente son: ", a, b, c, d, e)
print("la mediana es: " + str(c))
#hallar el promedio
promedio= (a+b+c+d+e)/5
print("el promedio es "+ str(promedio))
#hallar el promedio multiplicativo
prom_mult= (a*b*c*d*e)**(1/5)
print("el promedio multiplicativo es "+str(prom_mult))
#hallar la potencia del numero mayor elevado por el menor
potencia=a**e
print("la potencia del mayor numero elevado al numero menor es: " + str(potencia))
#hallar la raiz cubica del numero menor
raiz= e**(1/3)
print("la raiz cubica del menor numero es: " + str(raiz))
```
#####  8. Escriba un programa al que se le ingrese la frecuencia de una onda en hz y como salida arroje en que parte del espectro electromagnético se encuentra.

Para el octavo punto, se declaró una variable como flotante, se le dijo al usuario que ingresara una frecuencia en Hz, dado el valor que ingresara, se determinaría por medio de condicionales a cuál categoría pertence, y para aquello se tiene que cumplir uno de estos condicionales, y de este modo la consola mostrará el espectro magnético en el que se encuentra.

```python
F = float(input("Ingrese la frecuencia de la onda en Hz: "))
if F < 3e9:
    print("La onda se halla en la categoria de radio.")
elif F >= 3e9 and F < 3e11:
    print("La onda se halla en la categoria de microondas.")
elif F >= 3e11 and F < 4.3e14:
    print("La onda se halla en la categoria de infrarrojo.")
elif F >= 4.3e14 and F < 7.5e14:
    print("La onda se halla en la categoria de luz visible.")
elif F >= 7.5e14 and F < 3e17:
    print("La onda se halla en la categoria de ultravioleta.")
elif F >= 3e17 and F < 3e19:
    print("La onda se halla en la categoria de rayos X.")
else:
    print("La onda se halla en la categoria de rayos gamma.")
```

##### 9.Escriba un programa que reciba el nombre en minúsculas de un país de America y retorne la ciudad capital, si el país no pertenece al continente debe arrojar país no identificado.

Para 

```python
paisyCapital = {
    "argentina": "Buenos Aires",
    "bolivia": "La Paz",
    "brasil": "Brasilia",
    "canada": "Ottawa",
    "chile": "Santiago",
    "colombia": "Bogotá",
    "costa rica": "San José",
    "cuba": "La Habana",
    "ecuador": "Quito",
    "el salvador": "San Salvador",
    "estados unidos": "Washington D.C.",
    "guatemala": "Ciudad de Guatemala",
    "haiti": "Puerto Príncipe",
    "honduras": "Tegucigalpa",
    "jamaica": "Kingston",
    "méxico": "Ciudad de México",
    "nicaragua": "Managua",
    "panamá": "Ciudad de Panamá",
    "paraguay": "Asunción",
    "perú": "Lima",
    "puerto rico": "San Juan",
    "república dominicana": "Santo Domingo",
    "uruguay": "Montevideo",
    "venezuela": "Caracas"
}
pais = input("Ingrese el nombre del país (en minúsculas): ")
if pais in paisyCapital:
    print("La capital de", pais.capitalize(), "es", paisyCapital[pais])
else:
    print("País no identificado")
```

##### 10. Escriba un programa que dada una distancia calcule:

- El tiempo que le tomaría a la luz recorrer la distancia.
- El tiempo que le tomaría al sonido (en el aire) recorrer la distancia.
- El tiempo que le tomaría al vehiculo comercial más veloz recorrer la distancia.
- El tiempo que le tomaría a Bolt recorrer la distancia.

Para este algoritmo se declaró distancia como una variable flotante en esta se le pedía al usuario que ingresara dicho valor, teniendo encuenta el valor de distancia, las variables tiempoLuz, tiempoSonido, tiempoVehiculo, tiempoUsainBolt dependían del valor ingresado por el usuario para así calcular el valor de estos, se usó la siguiente formula de física para hallarlos:

$$t=d/v$$

Donde t, es el tiempo, d la distancia y v la velocidad, cada una de las variables ya mencionadas contaban con su repectiva velocidad, solo se requiere el valor de la distancia que el usuario fuera ingresara para calcular el tiempo, y finalmente la consola mostraría el tiempo que les tomaría.

```python
distancia = float(input("Ingrese la distancia en metros: "))
tiempoLuz = float(distancia /299792458)
tiempoSonido = float(distancia /343.2)
tiempoVehiculo = float(distancia/141.11)
tiempoUsainBolt = float(distancia/12.42)
print("El tiempo que tardaría la luz en recorrer la distancia es de: " + str(tiempoLuz) + " segundos.")
print("El tiempo que tardaría el sonido en recorrer la distancia es de: " + str(tiempoSonido) + " segundos.")
print("El tiempo que tarda el vehiculo comercial mas rapido en recorrer la distancia es de: " + str(tiempoVehiculo) +" segundos.")
print("El tiempo que tarda Usain Bolt en recorer la distancia es de: " + str(tiempoUsainBolt) + " segundos.")
```
