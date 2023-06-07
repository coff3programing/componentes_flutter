# ListView

![Dart](https://img.shields.io/badge/dart-%230175C2.svg?style=for-the-badge&logo=dart&logoColor=white)
![Flutter](https://img.shields.io/badge/Flutter-%2302569B.svg?style=for-the-badge&logo=Flutter&logoColor=white)

En Flutter, ListView.builder y ListView.separated son dos tipos de widgets que se utilizan para mostrar listas de elementos en una aplicación.

## ListView.builder

El widget ListView.builder se utiliza cuando se desea crear una lista de elementos con una estructura similar y una cantidad potencialmente grande de elementos. En lugar de construir todos los elementos de la lista de una vez, ListView.builder genera los elementos bajo demanda a medida que se desplaza por la lista, lo que mejora el rendimiento y ahorra recursos.

![list view](https://i.ytimg.com/vi/k1LxTsmAURU/maxresdefault.jpg)

El constructor ListView.builder toma una función de constructor de elementos llamada itemBuilder que se llama automáticamente cuando se necesita construir un elemento en la lista. Esta función toma un índice como argumento y devuelve el widget que representa ese elemento en la posición dada.

### Ejemplo

estamos construyendo una lista de 100 elementos donde cada elemento es representado por un widget ListTile con un título.

```Dart
ListView.builder(
  itemCount: 100, // Cantidad total de elementos en la lista
  itemBuilder: (BuildContext context, int index) {
    // Construye un elemento individual de la lista
    return ListTile(
      title: Text('Elemento $index'),
    );
  },
);
```

## ListView.separated

> El widget ListView.separated se utiliza cuando se desea mostrar una lista de elementos con separadores personalizados entre cada elemento. Puede ser útil cuando los elementos tienen diferentes estilos o cuando se desea agregar un espacio o un divisor visual entre ellos.

![List.separate](https://flutter.github.io/assets-for-api-docs/assets/widgets/list_view_separated.png)

El constructor ListView.separated toma tres funciones: itemBuilder, separatorBuilder y itemCount. itemBuilder es similar al utilizado en ListView.builder y se utiliza para construir cada elemento en la lista. separatorBuilder se utiliza para construir el separador entre cada elemento. itemCount especifica la cantidad total de elementos en la lista.

**_Ejemplo_**

En este ejemplo, estamos construyendo una lista de 100 elementos, donde cada elemento es representado por un widget ListTile, y utilizamos un Divider como separador entre ellos

```Dart
ListView.separated(
  itemCount: 100, // Cantidad total de elementos en la lista
  itemBuilder: (BuildContext context, int index) {
    // Construye un elemento individual de la lista
    return ListTile(
      title: Text('Elemento $index'),
    );
  },
  separatorBuilder: (BuildContext context, int index) {
    // Construye el separador entre los elementos
    return Divider();
  },
);
```

Conclusión:

> Ambos ListView.builder y
> ListView.separated
> son widgets muy útiles para crear listas dinámicas en Flutter,
> y ofrecen una forma eficiente y flexible de mostrar contenido en una aplicación.
