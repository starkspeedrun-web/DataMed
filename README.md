# DataMed - Sistema de Gestión Médica y Pacientes

## 📋 Descripción del Proyecto
**DataMed** es una plataforma integral diseñada para optimizar y modernizar la gestión de pacientes, citas médicas, expedientes clínicos y administración interna en centros de salud.

## 🎯 Objetivo
Facilitar el control operativo y la consulta de información médica mediante una interfaz centralizada, eficiente y segura que mejore la atención al paciente y reduzca la carga administrativa.

## ⚠️ Problema que Resuelve
La gestión tradicional en clínicas y consultorios suele enfrentar fragmentación de la información, duplicidad de registros, retrasos en la programación de citas e ineficiencia en el acceso al historial clínico de los pacientes. DataMed soluciona estas problemáticas centralizando los datos operativos y médicos bajo una arquitectura robusta y escalable.

---

## 🔥 Funcionalidades Principales
- **Gestión de Pacientes:** Registro, actualización de datos demográficos y consulta de historial médico.
- **Módulo de Citas Médicas:** Programación, reprogramación y cancelación de citas con asignación de doctores y especialidades.
- **Expediente Clínico Digital:** Registro de diagnósticos, recetas y notas de evolución médica.
- **Gestión de Usuarios y Roles:** Control de acceso para administradores, médicos y personal recepcionista.

---

## 🏗️ Arquitectura Seleccionada
El sistema está diseñado bajo el patrón de **Monolito Modular** (*Modular Monolithic Architecture*).
- **Justificación:** Permite mantener un único despliegue con límites lógicos claros entre módulos (Pacientes, Citas, Usuarios, Expedientes). Facilita el desarrollo inicial, simplifica las pruebas y permite una futura migración a microservicios si el volumen de datos lo requiere.

---

## 💻 Organización Frontend y Backend

### 🔵 Frontend (Capa de Presentación)
- **Responsabilidad:** Interfaz de usuario (UI) interactiva, validación de datos en el cliente y renderizado dinámico de vistas (paneles de control, formularios de registro y calendarios de citas).
- **Tecnologías:** HTML5, CSS3, JavaScript / React (o el framework seleccionado).

### 🟢 Backend (Capa de Lógica de Negocio y Datos)
- **Responsabilidad:** Procesamiento de reglas de negocio, autenticación/autorización de usuarios, gestión de la base de datos y validaciones del lado del servidor.
- **Tecnologías:** Node.js / C# / Python (según stack) y base de datos relacional (PostgreSQL / MySQL).

### 🔄 Comunicación Frontend / Backend
La comunicación entre el Frontend y el Backend se realiza mediante una **API RESTful** codificada en formato **JSON** sobre protocolo **HTTPS**. 
1. El Frontend realiza peticiones HTTP (`GET`, `POST`, `PUT`, `DELETE`) con cabeceras de autenticación (JWT).
2. El Backend procesa la solicitud, ejecuta la lógica correspondiente en la base de datos y responde con estados HTTP estandarizados (`200 OK`, `201 Created`, `400 Bad Request`, `401 Unauthorized`, etc.) y la carga útil en formato JSON.

---

## 🛠️ Herramientas Utilizadas
- **Control de Versiones y Gestión:** Git, GitHub (Repositories, Projects Kanban & Issues).
- **Modelado UML:** Visual Paradigm Online.
- **Documentación Técnica:** Markdown, Google Docs / PDF.

---

## 📈 Estado Actual del Proyecto
- **Fase Actual:** Cierre Técnico e Integración de Evidencias (Fase Inicial / Prototipado de Modelo).
- **Estatus:** Modelos UML definidos, arquitectura establecida, flujo de trabajo en Kanban estructurado y repositorio inicial configurado.
