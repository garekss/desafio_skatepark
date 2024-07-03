### Instalación de dependencias
`$ npm install`
### Consideraciones
Consideraciones:
- El sistema debe permitir registrar nuevos participantes.
- Se debe crear una vista para que los participantes puedan iniciar sesión con su correo
y contraseña.
- Luego de iniciar la sesión, los participantes deberán poder modificar sus datos,
exceptuando el correo electrónico y su foto. Esta vista debe estar protegida con JWT
y los datos que se utilicen en la plantilla deben ser extraídos del token.
- La vista correspondiente a la ruta raíz debe mostrar todos los participantes
registrados y su estado de revisión.
- La vista del administrador debe mostrar los participantes registrados y permitir
aprobarlos para cambiar su estado.

#### Base de datos


    CREATE DATABASE skatepark;
	  CREATE TABLE skaters (id SERIAL, email VARCHAR(50) NOT NULL, nombre
    VARCHAR(25) NOT NULL, password VARCHAR(25) NOT NULL, anos_experiencia
    INT NOT NULL, especialidad VARCHAR(50) NOT NULL, foto VARCHAR(255) NOT
    NULL, estado BOOLEAN NOT NULL);

![Captura de pantalla 2024-07-01 162629](https://github.com/garekss/desafio_skatepark/assets/159491346/64a682c5-f6e1-4d61-886f-692683e13096)

#### Administrador

![Captura de pantalla 2024-07-01 162522](https://github.com/garekss/desafio_skatepark/assets/159491346/4d5e7bf9-8a3c-4617-a4c6-122cf153733a)

#### Principal y estado

![Captura de pantalla 2024-07-01 162814](https://github.com/garekss/desafio_skatepark/assets/159491346/2d56065d-4ff6-422e-8710-128829fa4e84)




    
    
