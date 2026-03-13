# 🚀 Sistema de Gestión de Inventario (SIM) - Full Stack

Bienvenido a la solución del desafío técnico **"Seniority Mid - Full Stack"**.

Este repositorio contiene la implementación completa del **Sistema de Inventario Multisucursal (SIM)**, una plataforma moderna diseñada para gestionar sedes, productos y stock con un enfoque radical en la **mínima fricción operativa**.

---

## 🏗️ Arquitectura de la Solución

El proyecto está dividido en dos micro-aplicaciones independientes pero integradas:

1.  **Backend (Spring Boot 3.x):**
    *   Expone una API RESTful robusta.
    *   Gestiona la lógica de negocio y la integridad de datos.
    *   Utiliza **H2 Database** (en memoria) para persistencia rápida y volátil.
    *   [Ver detalles técnicos y arquitectura del Backend](https://github.com/jorgeobnd/backend/tree/master)

2.  **Frontend (Angular 16+):**
    *   Interfaz de Usuario reactiva y optimista.
    *   Diseñada con **Tailwind CSS** para una experiencia limpia y responsiva.
    *   Implementa patrones de UX para editar inventarios en tiempo real.
    *   [Ver detalles de UX y componentes del Frontend](https://github.com/jorgeobnd/frontend/tree/master)

---

## ⚡ Guía de Inicio Rápido (Local)

Para ejecutar la solución completa en tu máquina local, sigue estos pasos en orden:

### Paso 1: Levantar el Backend
El servidor debe estar corriendo para que el frontend pueda obtener datos.

```bash
cd backend
./mvnw spring-boot:run
# El servidor iniciará en http://localhost:8080
```

### Paso 2: Levantar el Frontend
En una nueva terminal:

```bash
cd frontend
npm install
ng serve
# La aplicación estará disponible en http://localhost:4200
```

¡Listo! Accede a `http://localhost:4200` para interactuar con el sistema.

---

## 🌐 Despliegue (Live Demo)

La aplicación ha sido desplegada y está lista para su revisión en línea. No es necesario instalar nada para probarla.

| Componente | URL de Acceso | Estado |
| :--- | :--- | :--- |
| **Frontend (App Principal)** | **https://frontend-six-sigma-27.vercel.app/** | 🟢 Online |
| **Backend (API)** | **https://backend-production-91eae.up.railway.app** | 🟢 Online |

> **Nota para el Evaluador:** El despliegue se realiza en [Plataforma, ej. Render/Railway]. El primer arranque puede demorar unos segundos debido al "cold start" del servicio gratuito.

---

## 📂 Estructura del Repositorio

```bash
.
├── backend/    # Código fuente Java/Spring Boot + Tests
├── frontend/   # Código fuente Angular + Estilos
└── README.md   # Este archivo (Guía General)
```

---

## ✅ Cumplimiento de Requerimientos

| Requerimiento | Estado | Implementación |
| :--- | :---: | :--- |
| **Administración de Sedes** | ✅ | CRUD completo (Crear, Editar, Eliminar) con validaciones. |
| **Catálogo Maestro** | ✅ | Gestión global de productos (Nombre, SKU, Precio). |
| **Control de Inventario** | ✅ | Edición de stock en tiempo real por sucursal. |
| **UX / Mínima Fricción** | ✅ | Interfaz de una sola pantalla, edición in-line, UI optimista. |
| **Responsive Design** | ✅ | Adaptable a móviles y tablets mediante Tailwind CSS. |
