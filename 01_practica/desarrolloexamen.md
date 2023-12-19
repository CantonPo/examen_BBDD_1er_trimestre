Nombre: Daniel Cantón Corpas

Fecha: 19/12/2023

He echo una pagina web con un input de texto y tres botones, añadir, borrar y sorteo.
El boton añadir mediante una funcion en java script añade elementos a una lista, borrar reinicia la lista
y sortea te da un elemento aleatorio entre todos los introducidos a la lista.

Tenemos dos archivos, ya que no he añadido archivo css por que le he adjuntado una libreria predefinida al html.

En el archivo index.html tenemos la extructura de pagina que hemos visto cientos de veces y que se abre sola mediante un atajo de teclado.
He añadido la libreria predefinida, un div class a la izquierda con la lista participantes y un contenedor que contiene el input de texto, los tres botones y el div del resultado del sorteo, todos con sus respectivas referencias para luego introducirlos en el archivo js, el cual también tiene abajo su referencia.

En el archivo js tenemos un let lista, con un JSON que recupera el valor del local storage y lo convierte en un elemento JavaScript, y este resultado se almacena en la variable lista. Luego comprueba si la lista es nula (esta vacia) si no es asi realiza el else. Con el bucle for creamos y almacenamos elementos en la lista de la clase ganador, los cuales llamaremos luego.
Ahora vamos llamando las funciones del html que tenemos en los botones, empezamos con añadir, coge un valor del html con id nanos, y se almacena en valor, crea un nuevo elemento con clase párrafo y lo agrega a la clase ganador, luego lo transformamos en una cadena con el json y actualiza el local storage.
La funcion borrar coge todos los elementos de la clase ganador y los borra, cogemos el local storage y borramos el elemto lista.
La funcion random coge un elemento aleatoriamente y la funcion sortear muestra este elemento aleatorio en el .resultadoSorteo