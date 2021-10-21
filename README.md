# Evaluacion-Practica-ProContacto

## Ejercicio 2 
Las siguientes preguntas están orientadas a la comprensión del protocolo HTTP. Son agnósticas al lenguaje de programación, la idea es comprender los conceptos del estándar:

 **1.	¿Qué es un servidor HTTP?**

 **2.	¿Qué son los verbos HTTP? Mencionar los más conocidos**

 **3.	¿Qué es un request y un response en una comunicación HTTP? ¿Qué son los headers?**

 **4.	¿Qué es un queryString? (En el contexto de una url)**

 **5.	¿Qué es el responseCode? ¿Qué significado tiene los posibles valores devueltos?**

 **6.	¿Cómo se envía la data en un Get y cómo en un POST?**

 **7.	¿Qué verbo http utiliza el navegador cuando accedemos a una página?**

 **8.	Explicar brevemente qué son las estructuras de datos JSON y XML dando ejemplo de estructuras posibles.**

 **9.	Explicar brevemente el estándar SOAP**

 **10.	Explicar brevemente el estándar REST Full**

 **11.	¿Qué son los headers en un request? ¿Para qué se utiliza el key Content-type en un header?**

## Ejercicio 3
Recomendamos previamente entender los conceptos de la sintaxis “json” antes de arrancar con los ejercicios.
Descargar el POSTMAN (aplicación para realizar request como cliente), adjuntando un screen de resolución para cada ítem:

**1.	Realizar un request GET a la URL: https://procontacto-reclutamiento-default-rtdb.firebaseio.com/contacts.json**

**2.	Realizar un request POST a la URL anterior, y con body:**
  ```
  {
  "name":"Tu nombre",
  "email":tunombre.tuapellido@procontacto.com.mx
  }
  ```
  Tip: (Marcar la opción “raw” como body)

**3.	Realizar nuevamente un request GET a la URL: https://procontacto-reclutamiento-default-rtdb.firebaseio.com/contacts.json**

**¿Qué diferencias se observan entre las llamadas el punto 1 y 3?** 
  Ahora mi información se encuentra disponible cuando realice el GET nuevamente. 

## Ejercicio 4
Solicitar usuario de Trailhead a ariel.tarsitano@procontacto.com.mx. Cambiar el idioma de Trailhead a inglés. Realizar los siguientes módulos de Trailhead:
●	[Fundamento de la plataforma Salesforce](https://trailhead.salesforce.com/content/learn/modules/platform_dev_basics?trailmix_creator_id=strailhead&trailmix_slug=prepare-for-your-salesforce-platform-developer-i-credential)

●	[Fundamentos de Apex y .NET](https://trailhead.salesforce.com/content/learn/modules/apex_basics_dotnet?trailmix_creator_id=strailhead&trailmix_slug=prepare-for-your-salesforce-platform-developer-i-credential)

●	[Modelado de datos](https://trailhead.salesforce.com/content/learn/modules/data_modeling?trailmix_creator_id=strailhead&trailmix_slug=prepare-for-your-salesforce-platform-developer-i-credential)

●	[Fundamentos y base de datos de Apex](https://trailhead.salesforce.com/content/learn/modules/apex_database?trailmix_creator_id=strailhead&trailmix_slug=prepare-for-your-salesforce-platform-developer-i-credential)

●	[Desencadenadores de Apex](https://trailhead.salesforce.com/content/learn/modules/apex_triggers?trailmix_creator_id=strailhead&trailmix_slug=prepare-for-your-salesforce-platform-developer-i-credential)

●	[Apex Integration Services](https://trailhead.salesforce.com/en/content/learn/modules/apex_integration_services)

Se recomienda usar el mismo Playground para todos los módulos solicitados. Excepto que se solicite crear uno nuevo en el enunciado del Módulo.
Para revisar la resolución de los módulos, compartir la URL del perfil público de Trailhead en una liga dentro del Readme.

## Ejercicio 5
Explicar que son conceptualmente, qué datos almacenan en forma estándar y cómo se relacionan el resto (algunos no se relacionan entre sí) cada uno de los siguientes objetos de Salesforce:

1.	Lead
2.	Account
3.	Contact
4.	Opportunity
5.	Product
6.	PriceBook
7.	Quote
8.	Asset
9.	Case
10.	Article

Los campos enumerarlos a través de una lista de texto en el Readme y las relaciones a través de un diagrama UML simple realizado con Drawio.

### Ejemplo de diagrama

Drawio: https://app.diagrams.net/
Que una cuenta tiene muchos contactos se representa de la siguiente manera:

Completar el resto de las relaciones agregando el resto de los objetos enumerados.
Exportar el diagrama de Drawio, subirlo al repositorio y agregarlo dentro del readme con la etiqueta para [linkear imágenes](https://stackoverflow.com/questions/14494747/how-to-add-images-to-readme-md-on-github).

Se puede usar el schema builder de salesforce para entender las relaciones.

https://trailhead.salesforce.com/content/learn/modules/data_modeling/schema_builder

## Ejercicio 6
Realizar las siguientes actividades sobre el Playground 1 del ejercicio 4:

A.	Consultar tu ID haciendo un GET con POSTMAN a este WS:
https://procontacto-reclutamiento-default-rtdb.firebaseio.com/contacts.json

B.	Agregar un campo al objeto Contact llamado idprocontacto de tipo texto de 255 caracteres. De la siguiente 
    No omitir poner el siguiente check cuando se crea el campo.
    
C.	Desarrollar un trigger para que cuando un usuario Modifica o Crea un contacto de Salesforce completando el campo generado el punto B con el ID del punto A, se invoque al Web Service con el idprocontacto obtenga los datos de email de la respuesta y actualice el campo email del contacto. Usar Playground 1. 

●	Para llamar web services desde un trigger ver este modulo de trailhead:https://trailhead.salesforce.com/content/learn/modules/apex_integration_services/apex_integration_rest_callouts

●	Para consultar un contacto en particular se puede agregar al ID al final de la URL como en este ejemplo: https://procontacto-reclutamiento-default-rtdb.firebaseio.com/contacts/-Ma6nC5l7n2nVal2zCyR.json

## Ejercicio 7

Responder las siguientes preguntas brevemente sobre:

### Soluciones de Salesforce

**A.	¿Qué es Salesforce?**
Salesforce es el CRM nº1 del mundo. ¿No está seguro de lo que es eso? ¡Se lo enseñaremos! De forma resumida, Salesforce empodera a las compañías con todo lo que necesitan para vender, ofrecer servicio y comercializar con sus clientes.

Trailhead lo empodera a usted con las aptitudes que esas compañías buscan al momento de una contratación. Además, la Trailblazer Community lo conecta con expertos de todo el mundo y con nuevas oportunidades profesionales.

**B.	¿Qué es Sales Cloud?**

**C.	¿Qué es Service Cloud?**

**D.	¿Qué es Health Cloud?**

**E.	¿Qué es Marketing Cloud?**

### Funcionalidades de Salesforce:

**A.	¿Qué es un RecordType?**

**B.	¿Qué es un ReportType?**

**C.	¿Qué es un Page Layout?**

**D.	¿Qué es un Compact Layout?**

**E.	¿Qué es un Perfil?**

**F.	¿Qué es un Rol?**

**G.	¿Qué es un Validation Rule?**

**H.	¿Qué diferencia hay entre una relación Master Detail y Lookup?**

**I.	¿Qué es un Sandbox?**

**J.	¿Qué es un ChangeSet?**

**K.	¿Para qué sirve el import Wizard de Salesforce?**

**L.	¿Para qué sirve la funcionalidad Web to Lead?**

**M.	¿Para qué sirve la funcionalidad Web to Case?**

**N.	¿Para qué sirve la funcionalidad Omnichannel?**

**O.	¿Para qué sirve la funcionalidad Chatter?**

### Conceptos generales:

**A.	¿Qué significa SaaS?**

**B.	¿Salesforce es Saas?**

**C.	¿Qué significa que una solución sea Cloud?**

**D.	¿Qué significa que una solución sea On-Premise?**

**E.	¿Qué es un pipeline de ventas?**

**F.	¿Qué es un funnel de ventas?**

**G.	¿Qué significa Customer Experience?**

**H.	¿Qué significa omnicanalidad?**

**I.	¿Qué significa que un negocio sea B2B?**

**J.	¿Qué significa que un negocio sea B2C?**

**K.	¿Qué es un KPI?**

**L.	¿Qué es una API y en qué se diferencia de una Rest API?**

**M.	¿Qué es un Proceso Batch?**

**N.	¿Qué es Kanban?**

**O.	¿Qué es un ERP?**

**P.	¿Salesforce es un ERP?**

