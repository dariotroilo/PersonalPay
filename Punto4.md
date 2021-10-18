Como parte del pipeline CI, arme 4 stages, con la siguiente descripcion:

stage "Building Proyect"
Realizo el pull del proyecto desde git y realizo la compilacion con Maven sin testear.

stage "Testing"
Realizo el test del build con maven utilizando el test incluido en el proyecto.

stage "Building Image"
Realizo la imagen docker con el tag latest

stage "Deploy image"
Realizo el push a Dockerhub de la imagen creada.