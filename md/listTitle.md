# ListView

![Dart](https://img.shields.io/badge/dart-%230175C2.svg?style=for-the-badge&logo=dart&logoColor=white)
![Flutter](https://img.shields.io/badge/Flutter-%2302569B.svg?style=for-the-badge&logo=Flutter&logoColor=white)

El widget ListTile en Flutter es un componente predefinido que se utiliza comúnmente para representar un elemento individual en una lista. Proporciona una estructura de diseño coherente y conveniente para mostrar contenido en una lista, como títulos, subtítulos, iconos y widgets secundarios.

![List Title](https://www.kindacode.com/wp-content/uploads/2020/10/Screen-Shot-2020-10-20-at-01.54.13.jpg)

El constructor ListTile tiene varios parámetros que permiten personalizar su apariencia y comportamiento:

- leading: es un widget opcional que se coloca en la parte izquierda del ListTile. Puede ser un Icon, una imagen u otro widget.
- title: es un widget obligatorio que representa el título principal del ListTile.
- subtitle: es un widget opcional que muestra un subtítulo o texto secundario debajo del título principal.
- trailing: es un widget opcional que se coloca en la parte derecha del ListTile. Puede ser un Icon, una imagen u otro widget.
- onTap: es una función opcional que se ejecuta cuando se toca el ListTile.
- selected: es un booleano opcional que indica si el ListTile está seleccionado o no. Esto puede afectar su apariencia visual.
- contentPadding: es un valor opcional que especifica el relleno interno del ListTile.

![Calendar](https://i.stack.imgur.com/KBzck.jpg)

### _*Ejemplo*_

Estamos creando un ListTile con un ícono a la izquierda, un título, un subtítulo y un ícono de flecha a la derecha. Además, hemos asociado una función al parámetro onTap, que se ejecutará cuando se toque el ListTile.

```Dart
ListTile(
  leading: Icon(Icons.person),
  title: Text('John Doe'),
  subtitle: Text('Software Developer'),
  trailing: Icon(Icons.arrow_forward),
  onTap: () {
    // Acción al tocar el ListTile
  },
);
```

> Conclusión:
> Es una forma eficiente y fácil de mostrar información estructurada en una lista en Flutter. Puedes personalizarlo y combinarlo con otros widgets para crear listas más complejas y atractivas en tus aplicaciones.
