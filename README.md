# Sistema de Registro de Tareas Colaborativas en Tiempo Real 🚀

Este proyecto es una aplicación web funcional desarrollada para la asignatura de **Tecnologías Emergentes** (7mo Semestre - Ingeniería de Sistemas) bajo la tutela del **Ing. Hermes Rodriguez Rivero**. La aplicación demuestra de forma práctica los conceptos de *Cloud Computing* mediante la implementación de un modelo de arquitectura moderna y serverless.

## 🎯 Objetivo General
Desarrollar una aplicación web funcional que integre un backend en tiempo real utilizando Supabase como servicio PaaS, gestionar el código fuente con Git y GitHub, y realizar su despliegue en producción mediante Vercel; aplicando los conceptos de Cloud Computing vistos en clase.

## 🛠️ Tecnologías y Herramientas Utilizadas (100% Gratuitas)
* **Backend (PaaS/BaaS):** Supabase (PostgreSQL + Realtime mediante WebSockets)
* **Hosting y Despliegue (PaaS):** Vercel (Hobby Tier)
* **Control de Versiones:** Git & GitHub (Repositorio Público)
* **Frontend:** HTML5, CSS3 (Diseño Responsivo) y JavaScript Moderno (Vanilla JS)
* **Editor de Código:** Visual Studio Code

## 🏗️ Arquitectura de la Aplicación
La aplicación sigue un modelo de arquitectura cloud serverless distribuida:
1. **Cliente (Navegador):** Carga los archivos estáticos desde la CDN global de Vercel e interactúa directamente con el SDK de Supabase.
2. **Capa de Datos e Interfaz (Supabase PaaS):** Gestiona las operaciones CRUD automáticas sobre la tabla de PostgreSQL mediante peticiones RESTful seguras.
3. **Sincronización Realtime:** Utiliza conexiones persistentes bi-direccionales de WebSockets para empujar cambios a todos los clientes conectados de forma inmediata cuando ocurre un evento (Insert/Update/Delete).

## 📂 Estructura del Proyecto
```text
tareas-cloud/
├── index.html       # Interfaz de usuario principal y carga de SDK (CDN)
├── style.css        # Estilos modernos, limpios y layout responsivo
├── app.js           # Lógica de negocio, conexión a Supabase y eventos Realtime
├── .gitignore       # Archivos y carpetas excluidos del control de versiones
└── README.md        # Documentación técnica completa del proyecto