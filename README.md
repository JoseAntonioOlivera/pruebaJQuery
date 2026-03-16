Paso 1. Añade el CDN de jQuery en la cabecera del documento.
Paso 2. Abre la etiqueta script al final del body y crea el bloque $(document).ready para asegurar que la página ha cargado.
Paso 3. Programa el botón Añadir Tarea (con id btnAnadir):
- Al hacer clic en el, lee el valor del input (id nuevaTarea) usando la funcion .val().
- Si el texto no está vacío, añade un nuevo elemento li al final de la lista (id listaTareas). Pista: investiga la funcion .append() de jQuery.
- Vacía el input despues de anadir la tarea para que quede limpio.
Paso 4. Programa que al hacer clic en cualquier tarea de la lista, se le aplique o quite la clase "completada" usando la funcion .toggleClass(). 
(Nota avanzada para el profesor: como los alumnos van a anadir elementos nuevos dinámicamente, explicales que deben usar $("#listaTareas").on("click", "li", function() {...}) en lugar de $("li").click() para que funcione en los elementos nuevos).
Paso 5. Programa el boton Ocultar Completadas (con id btnLimpiar):
- Al hacer clic, busca todos los elementos que tengan la clase "completada" y ocultalos usando un efecto visual como .fadeOut("slow").