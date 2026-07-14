
# Creación
Se crea a partir de la palabra reservada ==new==  y el nombre de la clase, esto crea una referencia al objeto que se guarda en la variable de la clase
```
Clase1 c = new Clase1();
String s = new String("Hola");
Object obj = new Object;
```

# Constructores
Se ejecuta durante la creación del objeto

```
Clase1 c = new Clase1(); //Al hacer la instancia con new, está mandandoa llamar ese constructor
```

# Destrucción de objetos
* Los objetos son destruidos por el ==Garbage Colector==
* Una vez pierde toda referencia a ese objeto, es candidato para llamar por el Garbage Colector
* El JVM llama a su método ==finalize()== una vez el objeto es elegido para su recolección ==Se puede llamar ese método 1 o ninguna vez==
![[Pasted image 20260713203102.png]]

* Como se puede ver en el ejemplo en la columna izquierda, se crean las referencias obj1 y obj2
* en la segunda columna obj1 iguala la ==referencia== a obj2 perdiendo su referencia original y siendo candidata para el Garbage colector
*  obj2 pierde su referencia, pero el objeto 2 sigue vivo porque obj1 sigue teniendo la referencia activa
