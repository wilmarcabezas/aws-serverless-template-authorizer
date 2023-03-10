# Bienvenidos al repositorio de AWS Serverless Authorizer 馃殌

Este repositorio contiene un ejemplo de c贸digo JavaScript para crear una funci贸n Lambda de AWS que maneje la autorizaci贸n de peticiones a una API Gateway.

## 驴Qu茅 hace este c贸digo?

El c贸digo consta de una funci贸n `generatePolicy` que toma como par谩metros el identificador del principal, el efecto (permiso o denegaci贸n) y el recurso al que se aplica la pol铆tica de autorizaci贸n. Esta funci贸n devuelve un objeto de respuesta de autorizaci贸n que incluye un documento de pol铆tica con la informaci贸n proporcionada y un contexto adicional opcional.

La funci贸n principal `handler` es la encargada de manejar las peticiones de autorizaci贸n que se env铆an a la funci贸n Lambda. Esta funci贸n toma un token de autorizaci贸n enviado en la petici贸n y, en funci贸n de su valor, devuelve una respuesta de autorizaci贸n permitiendo o denegando el acceso al recurso especificado en la petici贸n.

## 驴C贸mo usar este c贸digo?

1. Crea una funci贸n Lambda en AWS y config煤rala para que se ejecute este c贸digo.
2. Asocia la funci贸n Lambda a un recurso de API Gateway como un "authorizer" para manejar la autorizaci贸n de peticiones a la API.
3. Configura los valores de token de autorizaci贸n que deseas permitir o denegar en la funci贸n handler.
4. Env铆a peticiones a la API Gateway con un token de autorizaci贸n especificado en la cabecera de autorizaci贸n para comprobar el funcionamiento de la autorizaci贸n.
5. Si quieres aprender m谩s sobre c贸mo manejar la autorizaci贸n de peticiones a una API Gateway con funciones Lambda, 
puedes consultar la documentaci贸n oficial de AWS o los tutoriales en l铆nea.

隆Esperamos que este repositorio te sea de utilidad! 馃槉馃
