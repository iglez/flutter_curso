# Notas Dart

## Recursos

Dart pad donde juntamos con dart

[https://dartpad.dev/](https://dartpad.dev/)



## Notas dia 1
### Hola Mundo
```
void main() {
  
  String nombre = 'Ivan';
  
  print('Hola mi nombre es $nombre y estoy contento de utilizar Dart');
  
}

```

### Variable
```
void main() {
  
  int miNumero = 4;
  String palabra = 'cuatro';
  double pi = 3.1416;
  
  print('Este es un numero el cual es $miNumero y se lee como "$palabra" este es pi $pi');
  
  String nombre = 'Ivan Gonzalez Quitero';
  
  print(nombre[0]);
  print(nombre.toUpperCase());
  
  print(miNumero.isEven);
  
}
```

### Condiciones

```
void main() {

  bool esActivo = true;
  
  print(esActivo);
  
  if ( !esActivo ) {
    print('Es Activo');
  } else {
    print('No es activo');
  }
  
}
```


### Listas
```
 void main() {
    List<int> numeros = [1,2,3,4,5];
    print(numeros);
  
    // Agregando
    numeros.add(6);
    
//     numeros.add('siete');
//     numeros.add(true);
  
    print(numeros);
    
  
    // Comentarios
    // obtener un elemento
//     print(numeros[6]);
  
    // Error para mostrar tipos de datos
//   var nume = numeros[6];
//   String nume = numeros[6];
  
  List<int> opciones = List<int>(10);
  print(opciones);
  
  opciones[1] = 5;
  opciones[9] = 50;
  
  // No se puede agregar elemento (manipular la cantidad de elementos)
//   opciones.add(5);
  
  print(opciones);
  
}
```

### Mapas

```
void main() {
  
  Map<String, dynamic> persona = {
    'nombre': 'Ivan',
    'edad': 38,
    'soltero': false,
  };
  
  print( persona['nombre'] );
  print( persona['soltero'] );
  
  
  Map<String, dynamic> imagen = {
    'src': './img/imamgen.png',
    'nombre': 'fotoBonita',
    'h': 5,
    'w': 10,
  };
  
  
  print( imagen );
  print( imagen['src'] );
  print( imagen['nombre'] );
  
  
  print('${imagen['src']} ----> ${imagen['nombre']}'  );
  
}
```

### Funciones
```
void main() {
  print('Funciones');
  
  String saludo = saludar(texto: "Hellow", nombre: "ivan");
  
  print(saludo);
  
}

// String saludar({String nombre, String texto}){
//   return '$texto $nombre';
// }


// Arrow function
String saludar({String nombre, String texto}) => '$texto $nombre';

```

### Clases

```
void main() {
  // Clases
  
  Heroe wolverine = Heroe(nombre:'Logan', poder:'regeneracion');
  
//   wolverine.nombre = 'Logan';
//   wolverine.poder = 'regeneracion';
  
  print( wolverine );
  // print( wolverine.nombre );
}


class Heroe {

  String nombre;
  String poder;
  
//   Heroe(String nombre, String poder) {
//     this.nombre = nombre;
//     this.poder = poder;
//   }
  
  
//   Heroe({String nombre, String poder}) {
//     this.nombre = nombre;
//     this.poder = poder;
//   }
  
  Heroe({this.nombre, this.poder});
  
  String toString() => '$nombre con poder de $poder';
 
}```
