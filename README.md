# React Test

## Intro

Son dos carpetas: `api` y `ui`. La carpeta `api` contiene una aplicacion que devuelve una lista de usuarios. 


##Descripcion de los componentes

###App

Este componente se encarga de pedir la lista de usuarios a la API.
Tiene propiedades para determinar la cantidad de usuarios a pedir y el largo de la lista de autocompletado.

###UserSearchModal

Este componente se encarga de mostrar/ocultar el modal, en funcion de lo que el usuario elija.
Para los botones y el modal se utilizan componentes de la libreria 'Material UI'

###AutocompleteUserName

Es un textbox que despliega una lista de sugeridos en funcion del input que ingresa el usuario.
Se construyo utilizando el componente 'AutoComplete' de la libreria 'Material UI', al que se le setean las siguientes propiedades:

* hintText: texto que aparece antes de que el usuario ingrese la busqueda

* filter: algoritmo utilizado para realizar la busqueda
Se utiliza 'fuzzyFilter', que permite realizar una busqueda mas fluida y menos estricta

* dataSource: la lista de datos a filtrar
La obtiene en sus propiedades

* dataSourceConfig: especifica clave y valor de los datos a filtrar
En este caso tanto la clave como el valor es el nombre del usuario

* maxSearchResults: limita el largo de la lista desplegada
