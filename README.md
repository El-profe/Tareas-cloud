# Sistema de Registro de Tareas Colaborativas en Tiempo Real 🚀

Este proyecto es una aplicación web funcional desarrollada para la asignatura de **Tecnologías Emergentes** (7mo Semestre - Ingeniería de Sistemas) de la **UAB FIT**, bajo la tutela del **Ing. Hermes Rodriguez Rivero**. La aplicación demuestra de forma práctica los conceptos de *Cloud Computing* mediante la implementación de un modelo de arquitectura moderna, serverless y adaptativa.

## 🔗 Enlaces del Proyecto
* **Repositorio Oficial:** [https://github.com/El-profe/Tareas-cloud](https://github.com/El-profe/Tareas-cloud)
* **Aplicación en Producción (Vercel):** [https://tareas-cloud-6yrm.vercel.app/](https://tareas-cloud-6yrm.vercel.app/)

## 🎯 Objetivo General
Desarrollar una aplicación web funcional que integre un backend en tiempo real utilizando Supabase como servicio PaaS, gestionar el código fuente con Git y GitHub, y realizar su despliegue en producción mediante Vercel; aplicando los conceptos de Cloud Computing y metodologías ágiles de despliegues.

## 🛠️ Tecnologías y Herramientas Utilizadas
* **Backend (PaaS/BaaS):** Supabase (PostgreSQL + Realtime mediante WebSockets)
* **Hosting y Despliegue (PaaS):** Vercel (Hobby Tier con integración CI/CD nativa)
* **Control de Versiones:** Git & GitHub (Repositorio Público)
* **Frontend:** HTML5, JavaScript Moderno (Vanilla JS) y CSS3 con diseño futurista (*Cyberpunk Dark Mode / Glassmorphism*) de arquitectura responsiva.
* **Editor de Código:** Visual Studio Code

## 🏗️ Arquitectura de la Aplicación
La aplicación sigue un modelo de arquitectura cloud serverless distribuida:
1. **Capa de Cliente (Navegador):** Carga los archivos estáticos e interactivos desde la CDN global de Vercel y procesa la lógica adaptativa para computadoras y dispositivos móviles.
2. **Capa de Datos e Interfaz (Supabase PaaS):** Gestiona las operaciones CRUD automáticas sobre la tabla de PostgreSQL en la región de São Paulo mediante peticiones RESTful seguras.
3. **Sincronización Realtime:** Utiliza conexiones persistentes bi-direccionales de WebSockets para empujar cambios a todos los clientes conectados de forma inmediata cuando ocurre un evento (Insert/Update/Delete), garantizando concurrencia inmediata sin recargar la página.

## 📂 Estructura del Proyecto
```text
tareas-cloud/
├── index.html       # Interfaz de usuario principal y carga de SDK (CDN)
├── style.css        # Estilos futuristas, neón y layout responsivo adaptativo
├── app.js           # Lógica de negocio, conexión a Supabase y eventos Realtime
└── README.md        # Documentación técnica completa del proyecto