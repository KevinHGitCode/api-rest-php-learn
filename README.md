# Proyecto API REST en PHP


## Objetivo del Proyecto

Este proyecto tiene como propósito aprender a desarrollar APIs REST utilizando PHP. Está diseñado como un manual sencillo y práctico, con varias indicaciones en el código para facilitar su comprensión y reutilización.


## Requisitos del Entorno

Antes de comenzar, asegúrate de contar con:

- **PHP** instalado en tu sistema (cualquier versión compatible con PDO).
- **MySQL** para la base de datos.
- **Apache** o cualquier servidor que soporte PHP.
- **Thunder Client** (extensión de VS Code) o Postman para probar los endpoints.


## Configuración del Entorno

1. Configura las credenciales de la base de datos en el archivo `config/config.php`.
2. Ejecuta el archivo `.database/setup.sql` en tu servidor de MySQL para crear la base de datos y poblarla con datos de prueba. La base de datos tiene el nombre **`usersdb`**.
   
   **Nota:** Si ya existe una base de datos con el mismo nombre, esta será eliminada. Cambia el nombre en `setup.sql` y `config.php` si es necesario.


## Estructura del Proyecto

La estructura de carpetas y archivos es la siguiente:

```
./api-rest-php-learn
├── .database
│   └── setup.sql               # Script para crear la base de datos
├── api
│   ├── ep1-get-method.php      # Endpoint para GET
│   ├── ep2-post-method.php     # Endpoint para POST
│   ├── ep3-put-method.php      # Endpoint para PUT
│   ├── ep4-delete-method.php   # Endpoint para DELETE
│   ├── ep5-patch-method.php    # Endpoint para PATCH
│   ├── ep6-head-method.php     # Endpoint para HEAD
│   └── ep7-options-method.php  # Endpoint para OPTIONS
├── config
│   ├── config.php              # Configuración de la base de datos
│   └── connection.php          # Conexión a la base de datos
├── model
│   └── UserModel.php           # Modelo de datos para usuarios
└── README.md                   # Este archivo
```


<details>
<summary style="font-size: 14px;">
<i>Alternativa de Estructura del Proyecto</i>
</summary>

<br />
<p style="margin-bottom: 8px;">Otra propuesta para la estructura de la API REST:<p>

```
.
├── api-rest/
│   ├── create_client.php
│   ├── delete_client.php
│   ├── get_all_client.php
│   └── update_client.php
│
├── includes/
│   ├── Client.class.php
│   └── Database.class.php
│
└── sql/
    └── setup.sql
```
</details>

## Pruebas y Ejecución

- Usa **Thunder Client** o **Postman** para probar los endpoints.
- Cada archivo en la carpeta `api/` contiene un ejemplo funcional del método HTTP correspondiente.
- La base de datos generada con `setup.sql` incluye datos de prueba en un estado inicial ("estado cero") para facilitar la validación.
- Las propuestas de prueba para los endpoints se basan en esta configuración inicial.


## Licencia y Uso

Este proyecto es completamente abierto y puede ser utilizado por cualquier persona interesada. No se necesita licencia, ya que es un proyecto sencillo de aprendizaje.


## Créditos y Recursos

Este proyecto fue inspirado por los siguientes tutoriales:

- [Cómo crear una API Rest en PHP paso a paso - Video 1](https://youtu.be/QJfRtxxJ1TA)
- [api rest en php - Video 2](https://youtu.be/XcgSPDK_zzU)

