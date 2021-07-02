# TEST-FULLSTACK
#### Las siguientes instrucciones corresponden a los detalles para el test práctico que es necesario realizar como aspirante al puesto "Desarrollador FullStack" para integrarte al equipo de eCommerce de Grupo Xcaret

#
### Proyecto
##### Carrito de compras de Vehículos simple que lee una lista de productos (No la modifica) y ofrece un selector de productos, un carrito con las compras para hacer modificaciones y una pantalla de agradecimiento con un desglose lo comprado. 

#
##### BackEnd 
#
###### ***Requerido*
#
- Desarrollado utilizando Fastify.js(https://www.fastify.io/), con conexion al motor de Base de Datos MongoDB(se incluye en el repo el csv y json con los datos que deberan importar en la base de datos) para manejo de CRUD del carrito y la lectura de los productos.  

 - Debe validar mediante el uso de interfaces de TypeScript la estructura de los objetos que recibe y envía. 
 
 - Todo el desarrollo del backend, debe ser con TypeScript

###### ***Opcional*

 - Implementación de AJV para validar datos (Ejemplo un número máximo de productos) y Helmet para seguridad (Ejemplo simular cabecera para ocultar información).

 - Debe agregar por lo menos dos test unitarios.

##### Entrega Backend

- Generales:  

    - Limpieza (Indentación, comentarios) 

    - Simplicidad (Hacer más con menos código) 

    - Detalle 

###### ***Requerido*

- Repositorio en GitHub con las instrucciones de como ejecutarlo y la documentación que considere necesaria. 

###### ***Opcional*

- Todo el desarrollo de backend debe subirse a una plataforma como Heroku o firebase 

- Para la base de datos deberá subirse a mongo atlas, debera permitir el ingreso a cualquier IP a modo de prueba (en la practica esto no debe ser así, solo es por motivos de revisión del test)


##### FrontEnd 

###### ***Requerido*

 - Desarrollo utilizando Next.js, Redux y React se debe conectar al BackEnd e incluir las siguientes:  

###### - Funcionalidades 

-   Cambio de moneda. 

-   En cualquier página de la aplicación permitir cambiar la moneda desplegada. Se ofrecen dos monedas para los productos Pesos Mexicanos y dólares. 

-   La moneda actual debe contenerse en el Redux Store con un default de pesos. 

###### - Páginas 

 - Cotizador: Que desglose los productos disponibles y permita seleccionar el que quiera comprar la persona. 

    - Al cargar la página generar un identificador de carrito y almacenarlo en Redux Store. Queda a criterio de la persona como generará este identificador. 

    - Agregar el producto con un estatus de reservado y comunicar al usuario que su producto se agregó. 

    - No permitir agregar dos veces el mismo producto (comunicar al usuario que el producto ya lo tiene en su carrito). 

- Carrito de compra: Que despliegue los productos actualmente reservados para el identificador de carrito y permita modificar la cantidad y modelo en caso de aplicar de cada producto así como eliminar productos. 

    - Debe mostrar el desglose de precios y el total por el carrito de compra. 

    - Si no tiene modelos el producto no mostrar selector de modelo. 

    - Debe tener un formulario para capturar el nombre de la persona y este se debe guardar en el Store de Redux para mostrarlo posteriormente en el agradecimiento (Campo obligatorio). 

    - Contar con un botón de confirmar compra que marcará los productos con un estatus de comprado y enviará a la página de agradecimiento. 

    - En caso de que el carrito esté vacío mostrar un mensaje de carrito vacío, ocultar el botón de confirmar y tener una liga al cotizador. 

- Página de agradecimiento: Que despliegue un mensaje de agradecimiento y un resumen de la compra de la persona. 

    - Desplegar en el agradecimiento el nombre del cliente almacenado en Redux Store. 

    - Desplegar una tabla con los productos comprado. 

    - Contar con un botón de realizar nueva compra. 

###### ***Requerido* 

- Uso de React Hooks en componentes. 

- Uso de Tailwind para interfaz responsiva mobile y desktop 


###### ***Opcionales*

- Por lo menos 5 Test unitarios de componentes con Jest y Enzyme 


#### Entrega 

- Generales:  

    - Limpieza (Indentación, comentarios) 

    - Simplicidad (Hacer más con menos código) 

    - Detalle 

###### ***Requerido*

- Repositorio en GitHub con las instrucciones de como ejecutarlo y la documentación que considere necesaria. 

###### ***Opcional*
- El proyecto lo debera subir a alguna plataforma como github pages o heroku
