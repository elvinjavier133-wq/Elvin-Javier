# Mercado Abierto RD - Software Testing Report (Login)

##  Descripción del Proyecto
**Mercado Abierto RD** es una plataforma digital diseñada para que emprendedores y trabajadores del sector informal en la República Dominicana puedan comercializar productos y servicios de forma sencilla. La aplicación funciona como una solución móvil multiplataforma con arquitectura cliente-servidor.

Este repositorio documenta el proceso de testing realizado sobre el **módulo de Inicio de Sesión (Login)** para garantizar un acceso seguro a las cuentas de usuario.

---

##  Alcance de las Pruebas
Se realizaron pruebas funcionales para validar que el sistema procese correctamente las credenciales y maneje los errores de acceso de forma adecuada.

**Versión del Documento:** 0.1  
**Fecha de Pruebas:** 29/11/2025

---

##  Casos de Prueba (Test Cases)

| ID | Descripción | Resultado Esperado | Estado |
| :--- | :--- | :--- | :--- |
| **TC-001** | Inicio con usuario y contraseña correctos | Acceso concedido al panel principal | **Pass** |
| **TC-002** | Inicio con credenciales incorrectas | Mensaje de error y acceso denegado | **Pass** |
| **TC-003** | Correo válido y contraseña incorrecta | Rechazo de acceso y mensaje de validación | **Pass** |
| **TC-004** | Campos de texto vacíos | Mostrar mensajes de campos obligatorios | **Pass** |
| **TC-005** | Recuperación de contraseña | Envío de código de verificación al correo | **Fail** |

---

##  Registro de Bugs (Defectos)
Se identificó un fallo crítico durante el ciclo de pruebas:

### **BG-001: El sistema no envía el código de recuperación**
* **Severidad:** Alta (Bloquea la recuperación de cuenta)
