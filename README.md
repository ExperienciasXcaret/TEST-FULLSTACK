# TEST-FULLSTACK
#### Las siguientes instrucciones corresponden a los detalles para el test práctico que es necesario realizar como aspirante al puesto "Desarrollador FullStack" para integrarte al equipo de eCommerce de Grupo Xcaret

#
### Proyecto
##### Se requiere desarrollar un sitio de ecommerce que permita la compra de automóviles con los siguientes requerimientos:

- Los productos se deben consultar desde las apis desarrollados en el backend.
- El sitio debe permitir la selección de un modelo del producto, color.
- El precio del automóvil varía dependiendo el modelo.
- Se debe poder ingresar el monto del enganche del auto y las cuotas (de 12 hasta 60 meses).
- Se debe poder comprar el auto.
  - Se debe mostrar el resumen de la compra, modelo, color, precio.
  - Se debe dar clic en pagar y cargar el formulario de pagos.
  - ingresar una tarjeta con 16 dígitos. 
  - ingresar un cvv con 3 dígitos.
  - ingresar una fecha validar (si la fecha ya paso envía error en endpoint).
  - Se debe validar la tarjeta en el endpoint.
  - Si todo es correcto, se guarda la venta y se envía a la thank you page.

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

###### - Consideraciones 

    - No permitir agregar dos veces el mismo producto (comunicar al usuario que el producto ya lo tiene en su carrito). 

    - Debe mostrar el desglose de precios y el total por el carrito de compra. 

    - Si no tiene modelos el producto no mostrar selector de modelo.
  

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
- Imprimir la cotización del auto, con el modelo, color, precio, enganche y mensualidades (segun los meses seleccionados) y permitir la impresión del mismo.
