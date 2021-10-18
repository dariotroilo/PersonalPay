1- Este proyecto lo tenia del curso de Devops que estoy realizando y me pareció interesante para presentarlo, ademas que tenia el test incluido en el proyecto.
2- Herramientas utilizadas:
   - Github
   - VS Code
   - Dockerhub
   - jenkins
   - k3d
4- ver archivo punto4.md
9- Pipelines adjuntados con este documento
   El Dockerfile esta en el proyecto que utilicé, esta modificado para mi proyecto y subido a mi github.
   Con respecto a las dudas e inconvenientes...
   - Al utilizar aws se me estaban disparando los costos con las pruebas al dejar el cluster creado.
   - Por ese motivo, instale k3d en otra vm para realizar pruebas, sin pensar en los costos.
   - La mayor parte del tiempo, la utilicé en configurar los ambientes, permisos, certificados, etc etc
   - Los plugin de jenkins(kubernetes CD) presentan issues con k3d, alguna documentacion sugiere realizar downgrade a la V1.
   - En general mis mayores inconvenientes se dieron en la creacion de los ambientes.
   - En AWS tambien he tenido inconvenientes para otorgarle permisos al usuario para crear el cluster y desplegar. 

Repos:
- https://github.com/dariotroilo/spring-petclinic forked desde https://github.com/spring-projects/spring-petclinic
- https://github.com/dariotroilo/personal_CD este es el yaml para realizar el deploy en kubernetes k3d, parte del pipeline CD.
- https://hub.docker.com/repository/docker/dariotroilo/personalpay Imagen docker
