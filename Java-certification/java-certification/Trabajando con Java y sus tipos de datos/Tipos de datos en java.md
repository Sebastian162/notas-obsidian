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
+ Octal: **0453**
+ Hexadecimal: **0xAF7**
+ Binario: **0b100011**

Se puede usar el símbolo _ para representar un literal numérico 
```
int n = 2_345;
double d = 45.9_9;
```


