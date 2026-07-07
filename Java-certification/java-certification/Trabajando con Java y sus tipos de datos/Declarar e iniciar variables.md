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

