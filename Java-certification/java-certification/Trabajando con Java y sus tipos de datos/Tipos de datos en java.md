Primitivos: cualquier tipo de dato básico en java como, int, boolean,  etc
![[Pasted image 20260706215219.png]]
 
 ### Tabla de Tipos Primitivos en Java

| **Tipo Primitivo** | **Tamaño** | **Fórmula del Rango (Complemento a 2)**   | **Rango de Valores Exacto**                                | **Valor por Defecto** |
| ------------------ | ---------- | ----------------------------------------- | ---------------------------------------------------------- | --------------------- |
| **`byte`**         | 8 bits     | $-2^{7}$ a $2^{7} - 1$                    | `-128` a `127`                                             | `0`                   |
| **`short`**        | 16 bits    | $-2^{15}$ a $2^{15} - 1$                  | `-32,768` a `32,767`                                       | `0`                   |
| **`int`**          | 32 bits    | $-2^{31}$ a $2^{31} - 1$                  | `-2,147,483,648` a `2,147,483,647`                         | `0`                   |
| **`long`**         | 64 bits    | $-2^{63}$ a $2^{63} - 1$                  | `-9,223,372,036,854,775,808` a `9,223,372,036,854,775,807` | `0L`                  |
| **`char`**         | 16 bits    | $0$ a $2^{16} - 1$ _(No firma negativos)_ | `0` a `65,535` (Caracteres Unicode)                        | `'\u0000'`            |
| **`float`**        | 32 bits    | IEEE 754                                  | Precisión simple (aprox. 7 dígitos decimales)              | `0.0f`                |
| **`double`**       | 64 bits    | IEEE 754                                  | Precisión doble (aprox. 15 dígitos decimales)              | `0.0d`                |
| **`boolean`**      | _Variable_ | No aplica                                 | `true` o `false`                                           | `false`               |


Objeto: Todo tipo de objeto en java incluso strings ya que son objetos



# Literales
Prácticamente es el valor de la variable

### Literales enteros
Se pueden representar de la siguiente manera:
+ Decimal: **289**
+ Octal: **0453**  (Empieza por cero)
+ Hexadecimal: **0xAF7**     (Se aceptan las letras A,B,C,D,E,F)
+ Binario: **0b100011**

Se puede usar el símbolo _ para representar un literal numérico 
_Restricciones_
* No inicio
* No final
* Junto punto separador de decimales
```
int n = 2_345;
double d = 45.9_9;
```

Todo literal con punto es considerado ==Double== solo si se requiere que este tenga un valor en especifico como float, este se tiene que interpretar en el código
```
4.7f
```



# Conversiones de tipos
Existen dos tipos de conversión de tipos ==explícitas== e ==implícitas==

Son ==Implícitas== cuando no se requiere hacer uso de algún casting, son directas
```
 int x = 7;
 double z = x;
```

Son ==explícitas== cuando se requiere un casting para transformarlas
```
double r = 4.5f;
int x = (int)r; //Casting forzoso
```


**Regla de conversión implícita**
* El tipo de dato de destino debe ser mayor al de origen, existen algunas excepciones para esta regla
* Tipo de origen es numérico (cualquier tipo) y el destino es char
```
byte b = 5;
char n = b; //ERROR
``` 
* El tipo de destino es entero y origen decimal

``` 
double a = 5.5;
long l = a; // ERROR
``` 
_Siempre existirá la opción de hacer la conversión explícita_




# Tipos objeto 
* Son todos los objetos de cualquier clase Java (Los strings son objetos)
* No existe conversiones entre objetos y promitivos 
* 
