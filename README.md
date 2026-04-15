# 🖥️ Documentación de Laboratorio #2 de Desarrollo de Software 7 - Instalación de Laravel + Ejecución

Este documentación esta enfocada como guía de instalación y ejecución del framework Laravel, desde prerequisitos, comandos, ejecución y errores comunes.

## 📌 Introducción 

En la arquitectura MVC:
- **Modelos (Models):** Gestionan la lógica de datos y la interacción con la base de datos.
- **Vistas (Views):** Representan la interfaz de usuario.
- **Controladores (Controllers):** Actúan como intermediarios entre modelos y vistas.

El laboratorio consiste en la creación de un sistema básico de autenticación (login y registro), comprendiendo la estructura del proyecto y el flujo de desarrollo en Laravel.

---

## ⚙️ Requisitos Previos

Antes de ejecutar el laboratorio, asegúrate de contar con:

- PHP versión 8.0 o superior  
- Composer (última versión estable)  
- Laravel Installer o uso de:
  - `composer create-project`
  - `laravel new`
- Entorno de desarrollo:
  - XAMPP / WampServer / Laragon  
- Servidor web:
  - Apache o Nginx  
- Base de datos:
  - MySQL o MariaDB  
- Editor de código:
  - Visual Studio Code (recomendado)  
- Node.js y NPM (para manejo de dependencias frontend)  
- Sistema Operativo:
  - Windows / Linux / MacOS  

---

## 📦 Instalación y Configuración

### 1. Crear el proyecto Laravel

```bash
laravel new example-app
```

### 2. Configurar variables de entorno
Tendrás que configurar en el archivo .env:

```
DB_DATABASE=nombre_db
DB_USERNAME=root
DB_PASSWORD=
```

### 3. Instalar dependencias
Dentro del nuevo proyecto, deberás instalar las siguientes dependencias usando estos comandos en la terminal:

```bash
composer install
npm install
```

### 4. Generar clave de aplicación
Dentro del proyecto:

```bash
php artisan key:generate
```

### 5. Ejecutar migraciones
Dentro del proyecto:

```bash
php artisan migrate
```

### 6. Limpiar caché de configuración
Dentro del proyecto:

```bash
php artisan config:clear
php artisan config:cache
```

### 7. Ejecutar proyecto
Dentro del proyecto:

```bash
composer run dev
```

## 🔐 Instalación de Autenticación
Se utilizó Laravel UI para implementar login y registro:

```bash
composer require laravel/ui
php artisan ui bootstrap --auth
npm install
npm run dev
```

## 🗄️ Base de Datos
- Se utilizó MySQL como sistema gestor de base de datos.
- Configuración realizada en el archivo .env.
- Migraciones ejecutadas con:
  
```bash
php artisan migrate
```

📌 ¿Qué hacen las migraciones?
- Crean tablas en la base de datos.
- Permiten versionar la estructura.
- Se almacenan en database/migrations.
  
🔄 Comandos importantes:

```bash
php artisan migrate
php artisan migrate:rollback
```

## 🖼️ Resultados del Laboratorio

