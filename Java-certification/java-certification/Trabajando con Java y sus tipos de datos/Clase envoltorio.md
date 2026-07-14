Son utilizadas para acceder a las propiedades de los tipos de datos primitivos, la idea es encapsular tipos primitivos como objetos

| **Tipo Primitivo** | **Clase Envoltorio (Wrapper)**                        |
| ------------------ | ----------------------------------------------------- |
| `boolean`          | **`Boolean`**                                         |
| `byte`             | **`Byte`**                                            |
| `short`            | **`Short`**                                           |
| `int`              | **`Integer`** _(¡Cuidado con este cambio de nombre!)_ |
| `long`             | **`Long`**                                            |
| `float`            | **`Float`**                                           |
| `double`           | **`Double`**                                          |
| `char`             | **`Character`** _(¡Cuidado también con este!)_        |
|                    |                                                       |

¿Cómo se utilizan?
==Envolvimiento==

 # Encapsulación tipos primitivos como objetos
```
 Integer miValor = new Integer(200);
 Double db = new Double(1.1);
```

 Estos ejemplos ya son deprecados par alas nuevas versiones, lo nuevo sería
```
 Integer miValor = Integer.valueOf(200);
 Double db = Double.valueOf(1.1);
```

==Desenvolvimiento== manual para extraer su valor primitivo puro 
```
 int k = miValor.intValue(); //Regresa el 200 de nuestro envolvimiento anterior
 double f = db.doubleValue(); //Regresa el 1.1 de nuestro envolvimiento anterior
```


# Método estático para convertir Strings en tipo primitivo u objeto
```
 int p = Integer.parseInt("300");
 int n = Integer.parseInt("100011",2); //Regresa 35
 Integer num = Integer.valueOf("100011",2);
```

# Autoboxing / unboxing
Se puede asignar directamente el valor a la variable objeto
```
Integer x = 50; //Autoboxing
Double db = 2.5; //Autoboxing
```

Se puede obtener el valor primitivo directamente (unboxing)
```
int a = x; //Unboxing
Integer a = 31 //Autoboxing
a++; //Unboxing más autoboxing
```

# Inmutabilidad de los objetos
Los objetos de las clases envolotrios son inmultables, no se pueden modificar
```
Integer ent = 300; //Autoboxing
ent = ent + 100;  // Unboxing + autoboxing (Genera nuevo objeto)
```

![[Pasted image 20260713215426.png]]

___________________________________
# ==NOTAS==
Todo método que empieza con ==parse== devuelven un tipo primitivo
```
 int p = Integer.parseInt("300");
```

Métodos que empiezan con ==valueOf== devuelven un objeto envoltorio
```
 Integer miValor = Integer.valueOf(200);
```

Método que terminan con ==Value()== sacan el primitivo dentro del objeto
```
 Integer miValor = Integer.valueOf(200);  //Se crea envoltorio
 int k = miValor.intValue(); // Se saca el valor primitivo de envoltorio
```

