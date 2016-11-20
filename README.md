# MVC-MVP
Arquitecturas MVC-MVP

##**Tarea:** _Investigar más a detalle en que consiste la Arquitectura Model View Presenter y cómo se diferencia del Model View Controller_
___
la intención del MVC es separar una aplicación en tres partes fundamenales, pero de alguna manera relacionadas:

* _Modelo:_ Es quien hace referencia a los datos o a la representación de la información. El modelo puede estar ligado a la persistencia de la información. El modelo es el estado del negocio y la persistenca de ese estado.
* _Controlador:_ Representa la lógica del negocio. Las reglas que hacen al negocio.
* _Vista:_ Representa la interfaz con el usuario.

El patrón MVP permite separar la capa de presentación de la lógica, así, todo lo relacionado con cómo funciona la interfaz queda separado del cómo representarlo en pantalla. El MVP no es un patrón de arquitectura de aplicaciones, sólo se encarga de la capa de presentación.  

Para que una aplicación sea fácilmente extensible y mantenible necesita tener bien separadas sus capas. El MVP nos divide la aplicación en, al menos, tres capas distintas, pudiendo además testear cada una de ellas de forma independiente. Hay muchas variaciones de MVP y cada uno puede ajustar la idea del patrón a sus necesidades y a la forma en que se sienta más cómodo. El patrón varía sobre todo en función de la cantidad de responsabilidades que deleguemos en el presentador.

* _El presentador:_ Se encarga de actuar de intermediario entre la vista y el modelo. Recupera los datos del modelo y se los devuelve a la vista formateados. Pero a diferencia del MVC típico, también decide qué ocurre cuando se interactúa con la vista.

* _La vista:_ Contendrá una referencia al presentador. Lo único que hará la vista será llamar a un método del presentador cada vez que se realice una acción sobre la interfaz.

* _El modelo:_ En una aplicación con una buena arquitectura por capas, este modelo es la puerta de enlace a la capa de dominio o de lógica de negocio. Es suficiente verlo como el proveedor de los datos que queremos mostrar en la vista.
