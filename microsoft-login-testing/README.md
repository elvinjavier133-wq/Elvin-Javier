# Microsoft Authenticator – QA Testing  
 **Pruebas Funcionales y Negativas | MFA (Multi-Factor Authentication)**  

Este proyecto forma parte de mi portafolio como **QA Tester Junior**.  
El objetivo es validar funcionalidades esenciales de una aplicación de autenticación multifactor similar a Microsoft Authenticator, verificando seguridad, manejo de códigos, flujos de inicio de sesión y respuesta ante errores.

---

##  Objetivo del Proyecto  
Demostrar mis habilidades en:

- Diseño de casos de prueba  
- Pruebas funcionales  
- Pruebas negativas  
- Reporte de bugs  
- Documentación técnica de testing  
- Validación de seguridad en flujos MFA  

---

##  Alcance de las Pruebas

Las pruebas cubren:

- Registro y configuración inicial  
- Inicio de sesión  
- Autenticación multifactor (MFA)  
- Ingreso de códigos OTP/TOTP  
- Manejo de errores  
- Pruebas negativas  
- Validación de mensajes del sistema  

---

## Entorno de Pruebas

- Dispositivo: Redmi Note 14 Pro+ 5G  
- Sistema Operativo: Xiaomi HyperOS  
- Versión: Android 15  
- Conexión: Datos móviles  
- Estado del dispositivo: Batería estable  
- Dependencias: Servicio backend de autenticación, aplicación **Microsoft Authenticator**

---

## 📂 Casos de Prueba Incluidos

### TC-001 – Iniciar sesión con Microsoft  
Validar que el usuario pueda iniciar sesión correctamente usando su cuenta.

### TC-002 – Código de verificación vencido  
Confirmar que el sistema rechace códigos expirados y muestre el mensaje correcto.

### TC-003 – Código incorrecto  
Verificar que el sistema detecte un código inválido.

### TC-004 – Campo de código vacío  
Validar el manejo de un ingreso de código vacío.

###  TC-005 – Inicio de sesión profesional/educativo  
Inicio de sesión con cuenta institucional vinculada a Microsoft 365.

###  TC-006 – Cuenta personal en opción profesional/educativa  
El sistema debe bloquear este flujo.

###  TC-007 – Autenticación con OTP generado por la aplicación  
Validar login mediante código temporal válido (TOTP).

---

## 🐞 Bugs Reportados

### BG-001 – Mensaje incorrecto al ingresar código vencido  
- Severidad: Media  
- Prioridad: Media  
- Resultado actual: El sistema no muestra el mensaje correcto al ingresar un código expirado.  
- Caso de prueba relacionado: **TC-002**

---

## 🧑‍💻 Autor

**Elvin Javier Rosa**  
Proyecto personal – Portafolio QA Tester Junior

---

## 📎 Notas

Este proyecto fue creado con **fines educativos** para demostrar mis habilidades profesionales en aseguramiento de calidad de software.
