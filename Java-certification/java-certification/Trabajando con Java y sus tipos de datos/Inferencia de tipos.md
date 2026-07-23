La inferencia de tipos es la asignación de una variable sin tiparla, es una característica agregada en la versión 10.
El declarar las variables de este tipo no hace más rápida o lenta su ejecución.


```
Class Test {
	var elemento = 10; //Error de compilación
	void ejemplo() {
		var a = 10; //Correcto
		var datos = new ArrayList<Integer>(); //Correcto
		
		var data = null; //Error de compilación
		var b; //Error de compilación
		var x,y,z = 10 //Error de compilación
		
		
		//Es correcto hacerlo en interaciones, ya que estas son variables locales
		for(var i = 0; i < 10; i++){
			//Correcto
		}
		
		for(var x: datos){
			//Correcto
		}
	}
}
```



# Consideraciones
Solo se puede hacer para variables locales
No se puede declarar varias al mismo tiempo