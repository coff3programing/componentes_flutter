# ListView

![Dart](https://img.shields.io/badge/dart-%230175C2.svg?style=for-the-badge&logo=dart&logoColor=white)
![Flutter](https://img.shields.io/badge/Flutter-%2302569B.svg?style=for-the-badge&logo=Flutter&logoColor=white)

_HomeScreen_ y _AppRouter_ son dos conceptos relacionados en el desarrollo de aplicaciones en Flutter.

![homescreen](https://i.ytimg.com/vi/r_k1uBXSqkw/maxresdefault.jpg)

## HomeScreen

Se refiere a la pantalla principal de una aplicación. Es la pantalla inicial que se muestra cuando se abre la aplicación y generalmente contiene la interfaz de usuario principal y las funcionalidades principales de la aplicación.

**_Ojo👀_**

> La pantalla de inicio puede variar según la aplicación y sus requisitos. Puede contener widgets como barras de navegación, elementos de menú, listas, formularios, imágenes, texto, etc. Es el punto de entrada para que los usuarios interactúen con la aplicación y accedan a otras partes de la interfaz.

![home](https://i.ytimg.com/vi/IqFP7jY_enc/maxresdefault.jpg)

## AppRouter

Se refiere a un enrutador o manejador de rutas en una aplicación Flutter. Es una clase que se utiliza para gestionar las diferentes rutas y navegación entre pantallas en la aplicación.

![router](https://koenig-media.raywenderlich.com/uploads/2021/12/Navigator2Libraries-feature.png)

El enrutador de la aplicación tiene la responsabilidad de definir y gestionar las rutas de la aplicación, es decir, qué pantallas se muestran en respuesta a las interacciones del usuario, como hacer clic en un botón o seleccionar un elemento de menú.

## Detalles

El AppRouter normalmente utiliza un enfoque basado en rutas para la navegación, donde cada ruta está asociada a una pantalla específica en la aplicación. Al recibir una solicitud de navegación, el AppRouter se encarga de cambiar la pantalla actual a la nueva pantalla correspondiente a la ruta especificada.

La implementación de AppRouter puede variar dependiendo de las preferencias y necesidades del desarrollador. Puede utilizar enrutamiento basado en paquetes o enrutamiento declarativo utilizando bibliotecas como flutter_bloc, GetX o Provider para gestionar el estado de la navegación.

![dos](https://oflutter.com/wp-content/uploads/2021/02/organized-navigation-named-route-in-flutter-scaled.jpg)

> Conclusión:
> HomeScreen es la pantalla principal de una aplicación que muestra la interfaz de usuario principal, mientras que AppRouter es un enrutador que se utiliza para gestionar las rutas y la navegación entre las pantallas de la aplicación. Juntos, permiten la creación de aplicaciones con múltiples pantallas y una navegación fluida entre ellas.
