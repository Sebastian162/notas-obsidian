# Declaración
==tipo== *identificador*; --> ==int== *mivar*;
###### Declaración e inicialización
int p = 0;
###### Declaración múltiple
int a, b, c = 0;

# Identificadores

**Caracteres permitidos**
Cualquier combinación de letras y números, así como los caracteres **$** y **_**

**Restricciones**
+ Uso de palabras reservadas
+ Caracteres especiales como espacios, puntos, guiones medios, @, #, !
+ Números al inicio 
+ Solo usar el caracter ==_== al inicio, desde la versión 9 no es permitido



# Ámbito de las variables
¿Cómo son declaradas las variables?

A nivel clase, compartida por todos los métodos, son llamadas *atributo* o *campo*

A nivel método, solo se usan en el interior del método, son llamadas *locales*

Ejemplo

```
public class Mascota {
	int a; //Variable atributo
	int b; //Variable atributo
	
	public void metodo(){
		int a; //Variable local con el mismo nombre que variable atributo
		int z; //Variable local
		
		a = 10; //Acceso a variable local
		this.a = 5; // Acceso a variable atributo
	}
}
```

# Inicialización de variables
Las _variables atributo_ **SI** se inicializan por defecto ✔️
Las _variables locales_ **NO** se inicializan por defecto ❌

¿Cómo se inicializan?

* Byte, short, int, long: 0 (para long sería 0L)
* Float, double: 0.0f, 0.0d
* boolean: false;
* char:  '\u0000'; (carácter nulo)
* Objecto: null;

# Variables, objetos y tipos primitivos


| Tipo primitivo               | Objeto                                      |
| ---------------------------- | ------------------------------------------- |
| La variable contiene al dato | La variable contiene una referencia el dato |
| int i = 10;                  | ![[Ejemplo referencia objeto.png\|297]]<br> |


Diferencia objetos y primitivos
* Tipo primitivo: en una asignación cada variable tiene una copia del dato
```
int r = 10;
int n = r;
```
![[Pasted image 20260706210307.png|79]]
* Tipo objecto: Ambas variables apuntaran al mismo objecto sin que se cree una copia del mismo
```
Object ob = new Object();
Object nob = ob;
```
![[Pasted image 20260706210430.png|181]]

