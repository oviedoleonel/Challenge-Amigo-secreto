Este es un proyecto simple para realizar sorteos de "Amigo Secreto". Permite a los usuarios agregar una lista de nombres y luego seleccionar un ganador de forma aleatoria con solo un clic. El objetivo principal es fortalecer la lógica de programación utilizando JavaScript, HTML y CSS.

Estructura del Proyecto
El proyecto consta de los siguientes archivos principales:

index.html: Define la estructura y el contenido de la página web.

app.js: Contiene la lógica principal en JavaScript para gestionar la lista de amigos y el sorteo.

style.css: Proporciona los estilos visuales para la interfaz de usuario.

assets/: Carpeta que contiene las imágenes utilizadas en el proyecto.

index.html
El archivo HTML es la base de la aplicación.

Header: Un encabezado con un título principal y una imagen representativa.

Input Section: Una sección que contiene el campo de texto (<input>) donde se ingresan los nombres y el botón (<button>) para agregarlos.

Lista de Amigos: Una lista desordenada (<ul>) con el id="listaAmigos" que se usa para mostrar los nombres que se han agregado.

Resultado: Un contenedor (<ul>) con el id="resultado" que muestra el nombre del ganador del sorteo.

Botón de Sorteo: Un botón (<button>) con el onclick="sortearAmigo()" que inicia la función de sorteo.

Script: La etiqueta <script src="app.js" defer></script> enlaza el archivo de JavaScript y lo carga de manera diferida para garantizar que el HTML se renderice primero.

app.js
El archivo de JavaScript contiene toda la lógica de la aplicación.

listaDeAmigos: Un arreglo ([]) que almacena todos los nombres ingresados por el usuario.

agregarAmigo():

Obtiene el valor del campo de entrada.

Valida que el campo no esté vacío.

Si no está vacío, añade el nombre al arreglo listaDeAmigos.

Llama a las funciones mostrarHtml() y limpiarImput().

limpiarImput():

Borra el contenido del campo de texto de entrada para que el usuario pueda escribir un nuevo nombre.

mostrarHtml():

Actualiza la lista en la interfaz de usuario.

Recorre el arreglo listaDeAmigos y crea un elemento de lista (<li>) para cada nombre, agregándolo al HTML.

sortearAmigo():

Verifica que la lista de amigos no esté vacía.

Genera un índice aleatorio (Math.floor(Math.random() * listaDeAmigos.length)).

Selecciona un nombre del arreglo usando el índice aleatorio.

Muestra el nombre del ganador en la sección de resultado.

Uso
Abre el archivo index.html en tu navegador web.

Escribe el nombre de cada amigo en el campo de texto.

Haz clic en el botón "Añadir" después de cada nombre. La lista se actualizará en la página.

Cuando hayas agregado todos los nombres, haz clic en el botón "Sortear amigo" para ver quién es el ganador.
