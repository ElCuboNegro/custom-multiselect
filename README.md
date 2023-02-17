# Selección múltiple personalizada
Autor original: @davidvitora

Última actualización por @Juan Jose Alban el 17 de febrero de 2023

## Resumen
Permite mostrar casillas de verificación en un nodo del canal de chat web para que los usuarios puedan seleccionar múltiples opciones. Las selecciones se convierten en una cadena de texto y se pueden acceder fácilmente a través de la carga útil (payload).

## Casos de uso:
Agrega casillas de verificación para seleccionar varias opciones en lugar de utilizar una habilidad de selección que solo permite una de muchas opciones.
Cómo usar
Descargue el archivo .tgz

Cargue el archivo que descargó.

<img width="1203" alt="Screen Shot 2022-06-03 at 3 08 59 PM" src="https://user-images.githubusercontent.com/87815239/171948531-94876f07-6fc3-43cc-bb2b-e7db9eb7ff94.png">
Desempaquete el módulo personalizado.

<img width="1205" alt="Screen Shot 2022-06-03 at 3 12 21 PM" src="https://user-images.githubusercontent.com/87815239/171948659-bedff569-e5c0-427f-8924-7e34211cc3bb.png">
Encienda el módulo.

<img width="1206" alt="Screen Shot 2022-06-03 at 3 12 45 PM" src="https://user-images.githubusercontent.com/87815239/171948710-8afd8a7b-d0c5-4217-925d-047cb388e770.png">
Reinicie el servidor.

<img width="1205" alt="Screen Shot 2022-06-03 at 3 11 26 PM" src="https://user-images.githubusercontent.com/87815239/171948815-26579990-2515-4a5c-94b9-79a52af06091.png">
Vuelva a Github y copie el contenido de sendComponent.js.

<img width="1264" alt="Screen Shot 2022-06-03 at 4 12 36 PM" src="https://user-images.githubusercontent.com/87815239/171951342-72401103-75e4-4fa3-941f-f72b1e63db01.png">
Cree una nueva acción en Botpress y pegue el contenido de sendComponent.js.
Uploading Screen Shot 2022-06-03 at 4.18.04 PM.png…

Ajuste la pregunta.

Modifique el aspecto y la sensación de las casillas de verificación en src/views/lite/components/style.css.

Luego, vaya al nodo donde desea que aparezcan las casillas de selección múltiple y agregue la acción.

<img width="1204" alt="Screen Shot 2022-06-03 at 4 18 36 PM" src="https://user-images.githubusercontent.com/87815239/171951705-b9a42a7c-2d7b-44d6-a9f7-5b5026a4d346.png">
<img width="1205" alt="Screen Shot 2022-06-03 at 4 18 50 PM" src="https://user-images.githubusercontent.com/87815239/171951721-4164f125-d163-4029-8dc9-623e071a6dc9.png">

Los valores de lo que se seleccionó se almacenan como una cadena separada por comas en event.payload.text.

## Consejo
Si deseas tener múltiples selecciones múltiples únicas en tu chatbot, duplica la primera acción y renombra y edita la copia para cada selección múltiple única.