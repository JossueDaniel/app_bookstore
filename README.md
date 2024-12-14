# App_bookstore
El proyecto app_bookstore es una aplicación web que permite a los usuarios registrarse y autenticarse para realizar comentarios a los libros publicados por el administrador.

### Características
- Autenticación de usuario con un modelo personalizado
- Docker para crear un contenedor de la aplicación web
- Docker para crear un contenedor de la base de datos postgresql
- Implementación de "debug toolbar" para  debugear las funcionalidades al lado del cliente

## Requisitos previos
- Python 3.8 o superior
- Docker
- Docker compose
- Django 4.x

## Instalación

### 1. Clonar el repositorio
```bash
git clone https://github.com/JossueDaniel/app_bookstore.git
```

```bash
cd app_bookstore
```

### 2. Ejecutar docker compose
```bash
docker compose up -d
```

### 3. Aplicar migraciones a la base de datos
```bash
docker compose exec web python manage.py migrate
```

### 4. Crear usuario root
```bash
docker compose exec web python manage.py createsuperuser
```
### 5. Acceder al servidor de desarrollo
http://localhost:8000/

