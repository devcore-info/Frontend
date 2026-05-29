# ConneXtion Helpdesk - Frontend Client 🎨

Este repositorio contiene la interfaz cliente para la **Mesa de Ayuda de ConneXtion** (Sprint 1), desarrollada con **HTML5, CSS3 y JavaScript Vanilla**.

## 📁 Estructura del Proyecto

```text
frontend/
│
├── index.html           # Selector de Portales (Clientes / Soporte)
├── client-register.html # CU1 - Registro de Clientes [PENDIENTE]
├── client-login.html    # CU2 - Inicio de Sesión de Clientes [PENDIENTE]
├── support-register.html# CU7 - Registro de Personal Técnico [PENDIENTE]
├── support-login.html   # CU8 - Inicio de Sesión Administrativo [PENDIENTE]
└── css/
    └── styles.css       # Estilos globales de la aplicación (CSS Variables)
```

---

## 🔌 Integración con el Backend JAX-RS

Dado que el backend se comunica puramente en formato **JSON**, todas las peticiones fetch de los formularios deben apuntar al servidor REST local (NetBeans/Payara/Glassfish) utilizando la siguiente URL base:

`http://localhost:8080/Backend/resources/api/v1/...`

### Tabla de Endpoints Destino:
* **Registro de Cliente (CU1):** `POST /Backend/resources/api/v1/clients/register`
* **Inicio de Sesión de Cliente (CU2):** `POST /Backend/resources/api/v1/clients/login`
* **Registro de Soporte (CU7):** `POST /Backend/resources/api/v1/support/register`
* **Inicio de Sesión de Soporte (CU8):** `POST /Backend/resources/api/v1/support/login`

---

## 🚀 Cómo ejecutar localmente

Puedes levantar un servidor HTTP simple para servir los archivos estáticos utilizando NodeJS:

1. Asegúrate de tener NodeJS instalado.
2. Abre la terminal en este directorio y ejecuta:
   ```bash
   npx serve .
   ```
3. O bien, abre el proyecto en VS Code y utiliza la extensión **Live Server**.
