# Bienvenidos al repositorio de AWS Serverless Authorizer 🚀

Este repositorio contiene un ejemplo de código JavaScript para crear una función Lambda de AWS que maneje la autorización de peticiones a una API Gateway.

## ¿Qué hace este código?

El código consta de una función `generatePolicy` que toma como parámetros el identificador del principal, el efecto (permiso o denegación) y el recurso al que se aplica la política de autorización. Esta función devuelve un objeto de respuesta de autorización que incluye un documento de política con la información proporcionada y un contexto adicional opcional.

La función principal `handler` es la encargada de manejar las peticiones de autorización que se envían a la función Lambda. Esta función toma un token de autorización enviado en la petición y, en función de su valor, devuelve una respuesta de autorización permitiendo o denegando el acceso al recurso especificado en la petición.

## ¿Cómo usar este código?

1 .Crea una función Lambda en AWS y configúrala para que se ejecute este código.
2. Asocia la función Lambda a un recurso de API Gateway como un "authorizer" para manejar la autorización de peticiones a la API.
3. Configura los valores de token de autorización que deseas permitir o denegar en la función handler.
4. Envía peticiones a la API Gateway con un token de autorización especificado en la cabecera de autorización para comprobar el funcionamiento de la autorización.
5. Si quieres aprender más sobre cómo manejar la autorización de peticiones a una API Gateway con funciones Lambda, 
puedes consultar la documentación oficial de AWS o los tutoriales en línea.

¡Esperamos que este repositorio te sea de utilidad! 😊🤓
