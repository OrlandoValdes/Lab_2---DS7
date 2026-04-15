# Documentación de Laboratorio #2 de Desarrollo de Software 7 - Instalación de Laravel + Ejecución

Este documentación esta enfocada como guía de instalación y ejecución del framework Laravel, desde prerequisitos, comandos, ejecución y errores comunes.

## Introducción 

En la arquitectura MVC:
- **Modelos (Models):** Gestionan la lógica de datos y la interacción con la base de datos.
- **Vistas (Views):** Representan la interfaz de usuario.
- **Controladores (Controllers):** Actúan como intermediarios entre modelos y vistas.

El laboratorio consiste en la creación de un sistema básico de autenticación (login y registro), comprendiendo la estructura del proyecto y el flujo de desarrollo en Laravel.

---

## Requisitos Previos

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
