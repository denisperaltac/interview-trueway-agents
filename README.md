# Entrevista Técnica Trueway Agents

Esta entrevista técnica busca evaluar conocimientos básicos acerca de React JS y CSS.

Paso 1: En la carpeta src crear dos nuevos archivos: - Home.jsx - HomeControl.jsx

Paso 2: En HomeControl.jsx deberemos crear un componente que contenga una funcion que realice una llamada al siguiente endpoint: "https://test.truewayrealtorsapi.com/getListing"
Esta llamada se realizara una vez al iniciar el componente y deberá incluir una query llamada "ListingId" y su valor debe ser almacenado en un Estado denominado "listingId" cuyo valor inicial sera: "RX-12346123|2"
Luego de realizar la llamada se debera pasar la respuesta a un nuevo estado denominado properties.
Además deberemos manejar el error por consola y setear el estado de properties a su valor inicial.
Por último deberemos retornar el componente Home.jsx y pasarle como parametro el estado que contiene nuestras propiedades.

Paso 3: En Home.jsx deberemos crear un componente que contenga el titulo "Mis Propiedades" seguido de una tabla en la cual mostraremos 4 columnas que seran las siguientes:

Images - Precio - Baños - Dormitorios y sus valores serán respectivamente: {properties.images.L[0].M.link.S} {properties.OriginalListPrice.N} {properties.BathroomsFull.N} {properties.BedroomsTotal.N}

Paso 4: Agreramos un input de tipo texto el cual deberá modificar el valor de nuestro estado "listingId" seguido de un botón que ejecutará nuestra funcion para obtener propiedades. El boton deberá estar deshabilitado si el valor del largo de listingId es menor a 3.

Paso 5: En caso de introducir un valor incorrecto para listingId y ejecutar la función para buscar propiedades, deberemos manejar el error relizando un renderizado condicional de nuestra tabla y en caso de que no venga ninguna propiedad en nuestro llamado deberemos mostrar un mensaje de error como por ejemplo "No pudimos encontrar ninguna propiedad con el siguiente listingId ."

Paso 6: Utilizar estilos css en linea para mejorar el aspecto general de nuestro componente.
