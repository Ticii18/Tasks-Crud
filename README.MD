# CRUD TASKS BACKEND

Este proyecto es una API para la gestión de tareas, construida con Node.js, Express y MySQL. Proporciona operaciones CRUD básicas para la administración de tareas.

## Tecnologías Utilizadas

- **Node.js**: Entorno de ejecución para JavaScript del lado del servidor.
- **Express**: Framework para construir aplicaciones web en Node.js.
- **mysql2**: Driver nativo para interactuar con bases de datos MySQL.
- **express-validator**: Dependencia para las validaciones.
- **TailwindCSS**: Dependencia para los estilos del frontend.

## Instalación

1. Clona este repositorio:

    git clone https://github.com/Ticii18/crud-tasks-backend.git

2. Navega al directorio del proyecto:

    cd crud-tasks-backend

3. Instala las dependencias:

    - **npm install express morgan mysql2 express-validator**
    - **npm install -D tailwindcss postcss autoprefixer**
    

4. Configura la base de datos MySQL. Asegúrate de tener una base de datos creada y actualiza los detalles de conexión en el archivo de configuración.

## Base de Datos

1. Crea una base de datos MySQL llamada `tasks_db`:

    ```sql
    CREATE DATABASE tasks_db;
    ```

2. Crea una tabla llamada `tasks` con las siguientes columnas:

    ```sql
    CREATE TABLE tasks (
        id INT AUTO_INCREMENT PRIMARY KEY,
        title VARCHAR(255) NOT NULL,
        description TEXT,
        isComplete BOOLEAN DEFAULT FALSE
    );
    ```

## Ejecución

Para iniciar el servidor, utiliza el siguiente comando:

    cd backend/integrador (npm run dev)

    cd ../../frontend (npm run dev)

El servidor escuchará en el puerto especificado en la configuración.

## Uso del Frontend

- **Agregar una Tarea**: Usa el formulario para agregar una nueva tarea con un título, descripción y si está completada o no.
- **Visualizar Tareas**: Las tareas agregadas se mostrarán en la lista de tareas.
- **Editar una Tarea**: Haz clic en el botón "Editar" junto a la tarea que deseas modificar.
- **Eliminar una Tarea**: Haz clic en el botón "Eliminar" junto a la tarea que deseas borrar.

## Licencia

Este proyecto está bajo la Licencia MIT - mira el archivo LICENSE para más detalles.
