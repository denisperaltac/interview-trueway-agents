# Entrevista Técnica Trueway Agents
Esta entrevista técnica busca evaluar conocimientos básicos acerca de React JS y CSS.

## Paso 1
En la carpeta src, crea dos nuevos archivos:

1.Home.jsx
2. HomeControl.jsx

## Paso 2
En HomeControl.jsx:

1. Crea un componente que contenga una función que realice una llamada al siguiente endpoint: https://test.truewayrealtorsapi.com/getListing.
2. La llamada se realizará una vez al iniciar el componente y deberá incluir una query llamada ListingId.
3. El valor inicial de ListingId será almacenado en un estado denominado listingId con el valor inicial: "RX-12346123|2".
4. Después de realizar la llamada, guarda la respuesta en un nuevo estado denominado properties.
5. Maneja cualquier error imprimiéndolo en la consola y reseteando el estado properties a su valor inicial.
6. Retorna el componente Home.jsx y pásale como parámetro el estado que contiene nuestras propiedades.

## Paso 3
En Home.jsx:

1.Crea un componente que contenga el título "Mis Propiedades".
2. Añade una tabla con 4 columnas:
Images - {properties.images.L[0].M.link.S}
Precio - {properties.OriginalListPrice.N}
Baños - {properties.BathroomsFull.N}
Dormitorios - {properties.BedroomsTotal.N}

Paso 4
1. Añade un input de tipo texto que modifique el valor del estado listingId.
2. Añade un botón que ejecutará la función para obtener propiedades.
3. El botón deberá estar deshabilitado si el valor de la longitud de listingId es menor a 3.

Paso 5
1. Si se introduce un valor incorrecto para listingId y se ejecuta la función para buscar propiedades, maneja el error realizando un renderizado condicional de la tabla.
2. Si no se encuentra ninguna propiedad con el listingId proporcionado, muestra un mensaje de error como: "No pudimos encontrar ninguna propiedad con el siguiente listingId."
   
Paso 6
Utiliza estilos CSS en línea para mejorar el aspecto general de tu componente.

