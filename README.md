# números y números repo #3
`hi, again, everyone. this is my second repo, sincerely i hate pseudocoding, it's like quite boring and a little bit complicated, but well, it is what it is.`

##### *first part* 

###### so, let's start w/ pseudocode:

    clase primo hasta n 
    inicio 
      algoritmo principal 
      inicio 
        real i, n, 
        entero i, n, 
        i = 2
        n = 0 
        primos = [ ]
        imprimir “Escriba hasta qué número quiere que se cuenten los números primos”
        leer n
        mientras i ≤ n : 
          si i % 2 ≠ 0 : 
            num_primo = True
            para j en primos [1 :  ] :
          si i % j == 0 :
            num_primo = False
            romper
        si num_primo = True :
          agregamos a primos
        i += 1
        fin mientras
        imprimir (primos)
      fin algoritmo principal 
    fin
----

###### now, mermaid:

```mermaid
   graph TD;
   A[Clase Primo hasta n ] --> B[inicio] --> C[Algoritmo Principal] --> D[inicio] --> E[real i, n
    i : entero
    n : entero
    i = 2
    n = 0
    primos = ] --> F[Escriba hasta qué numero quiere que se cuenten los nuúmeros primos] --> G[leer n] -->
    H[mientras i <= n : ]--> I{si i % 2 != 0 :} --> J[num_primo = True]--> k[para j en primos 1 : ] --> L[si i % j == 0 :]--> M[num_primo = False
    romper]
    I --> H
    M --> N[si num_primo = True: ] --> O[agregamos a primos] --> P[i += 1] --> Q[fin mientras] --> R[imprimir primos] --> S[fin algoritmo principal] --> T[fin]
    P --> H
```

----

##### *second part*

##### let's start w/ pseudocode for this one:
    clase raíz cuadrada exacta
    inicio 
      algoritmo principal 
      inicio 
        real raiz_cuadrada(numero)
        raiz_cuadrada(numero) = 
        digitos = [ ]
        numero_cadena = str(numero)
        para i en rango (0, longitud(numero_str), 2) :
          añadir digitos a digitos(numero_str[i : i+2]
          raiz = " " 
          resto = 0
        para digito en digitos :
          cifra = 0
          mientras (cifra * cifra <= entero(digito) + resto:
            cifra += 1 
          resto = entero(digito) + resto) - cifra * cifra
          raiz += str(cifra)
        retornar float(raiz)
        numero = x
        raiz = raiz_cuadrada(numero)
        imprimir (`La raíz cuadrada de ${x} es ${raiz}`)
      fin algoritmo principal 
    fin

#### now, mermaid: 

```mermaid
  graph TD;
  A(Inicio) --> B(Algoritmo principal)
  B(Algoritmo principal) --> C(Función raiz_cuadrada_numero)
  C(Función raiz_cuadrada_numero) --> D(Convertir numero a cadena)
  D(Convertir numero a cadena) --> E(Ciclo para obtener dígitos pares)
  E(Ciclo para obtener dígitos pares) --> F(Calcular cifra)
  F(Calcular cifra) --> G(Actualizar resto)
  G(Actualizar resto) --> H(Agregar dígito a la raíz)
  H(Agregar dígito a la raíz) --> I(Ciclo para obtener dígitos pares)
  I(Ciclo para obtener dígitos pares) --> J(Convertir raíz a flotante)
  J(Convertir raíz a flotante) --> K(Asignar valor a la variable numero)
  K(Asignar valor a la variable numero) --> L(Llamar a la función raiz_cuadrada)
  L(Llamar a la función raiz_cuadrada) --> M(Imprimir resultado)
  M(Imprimir resultado) --> N(Fin)
  
  B(Algoritmo principal) --> O(Fin algoritmo principal)
  C(Función raiz_cuadrada_numero) --> P(Fin función raiz_cuadrada)
```
