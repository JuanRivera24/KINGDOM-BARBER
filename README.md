======================================================================
              PROYECTO INTEGRADOR: KINGDOM BARBER
======================================================================

Integrantes:
- Alejandro Urrego
- Andrés Vallejo
- Juan Manuel Rivera

Institución:
Institución Técnica CESDE

Fecha:
2025

======================================================================
1. INTRODUCCIÓN Y VISIÓN GENERAL
======================================================================

1.1 Resumen del Proyecto
------------------------
El proyecto **Kingdom Barber** nace como una plataforma digital integral, 
diseñada para transformar y modernizar la gestión de barberías.  
Su objetivo es ofrecer una solución robusta que simplifique la administración 
de citas, enriquezca la interacción con el cliente y proporcione herramientas 
avanzadas para la toma de decisiones.  

El ecosistema se compone de aplicaciones que trabajan de manera sinérgica:
- **API Central (Node.js + Express):** Cerebro de la operación, gestiona la lógica 
  de negocio y los datos.
- **Plataforma Web (Next.js):** Interfaz para clientes y barberos, optimizada 
  para la reserva de servicios.
- **Panel de Gestión y Análisis (Python + Streamlit):** Herramienta administrativa 
  con análisis de datos e Inteligencia Artificial.
- **Aplicación Independiente (Java + Spring Boot):** Sistema adicional autónomo 
  que no depende de la API Central.

1.2 Planteamiento del Problema
------------------------------
La gestión tradicional de barberías enfrenta limitaciones en la era digital:  
procesos manuales, comunicación ineficiente y carencia de análisis de datos.  
Esto disminuye la eficiencia operativa y afecta la experiencia del cliente, 
que hoy exige comodidad, seguridad y personalización.  

1.3 Solución Propuesta
----------------------
**Kingdom Barber** responde a estos desafíos con una plataforma unificada que 
digitaliza y optimiza las operaciones.  

Características clave:
- Gestión de reservas en línea.
- Catálogo de servicios con opciones personalizadas.
- Comunicación directa con clientes.
- Panel administrativo con análisis de datos e IA para reportes y marketing.

======================================================================
2. OBJETIVOS DEL PROYECTO
======================================================================

2.1 Objetivo General
--------------------
Mejorar la eficiencia operativa de las barberías mediante la digitalización 
de la gestión de reservas y la comunicación con clientes, ofreciendo una 
experiencia personalizada que aumente su satisfacción.

2.2 Objetivos Específicos
--------------------------
- **Seguridad y Acceso:** Desarrollar un sistema de autenticación robusto.  
- **Usabilidad y Navegación:** Crear interfaces intuitivas y responsivas.  
- **Gestión de Reservas:** Implementar un sistema completo de citas con 
  calendarios interactivos.  
- **Experiencia Personalizada:** Ofrecer catálogos y servicios adaptados 
  al cliente.  

======================================================================
3. ARQUITECTURA GENERAL DEL SISTEMA
======================================================================

3.1 Diseño de la Arquitectura
-----------------------------
El proyecto adopta una **arquitectura de servicios desacoplados**, 
donde cada módulo cumple una responsabilidad única.  

- **API Central (Node.js + Express):** Única fuente de verdad.  
- **Frontend Cliente (Next.js + React):** Capa de presentación que consume la API.  
- **Panel de Gestión (Python + Streamlit):** Se conecta a la API para análisis y reportes.  
- **Aplicación Independiente (Spring Boot):** Proyecto autónomo que no interactúa 
  con la API Central.  

3.2 Flujo de Datos
------------------
Ejemplo: Creación de una cita en la plataforma web.  

1. El cliente llena el formulario en **Next.js**.  
2. El frontend empaqueta los datos y los envía en formato JSON al endpoint 
   `/nuevas_citas` de la **API Central**.  
3. El servidor en **Node.js** valida y guarda la información en 
   `nuevas_citas.json`.  
4. La API responde con un **201 Created** y el objeto creado en JSON.  
5. El frontend actualiza la UI mostrando la cita confirmada.  

======================================================================
4. MÓDULOS DEL PROYECTO
======================================================================

4.1 Módulo 1: API Central (Node.js + Express)
---------------------------------------------
- **Descripción:** Núcleo del sistema. Gestiona lógica de negocio, 
  datos en JSON y seguridad.  
- **Funciones:**  
  - Endpoints CRUD para clientes, barberos, sedes, servicios, citas y galería.  
  - Subida de archivos con Multer.  

4.2 Módulo 2: Plataforma Web (PI_WEB2)
--------------------------------------
- **Descripción:** Interfaz visible para clientes y barberos, desarrollada 
  con Next.js, React y TypeScript.  
- **Funciones:**  
  - Reservas conectadas a la API Central.  
  - Catálogo de servicios y sedes.  
  - Panel de barberos para gestionar agenda y galería.  

4.3 Módulo 3: Panel de Gestión (PI_NTP)
---------------------------------------
- **Descripción:** Aplicación estratégica en Python con Streamlit.  
- **Funciones:**  
  - Dashboard interactivo con KPIs y filtros.  
  - Gestión de citas históricas.  
  - Asistente de IA para reportes, análisis y marketing.  

4.4 Módulo 4: Aplicación Independiente (PI_MOVIL2)
--------------------------------------------------
- **Descripción:** Proyecto autónomo en Spring Boot (Java) y VanillaJS.  
- **Nota:** No se integra con la API Central.  

======================================================================
5. STACK TECNOLÓGICO CONSOLIDADO
======================================================================

| Capa                  | Tecnología                  | Propósito                          |
|-----------------------|-----------------------------|------------------------------------|
| Backend (API Central) | Node.js, Express.js         | Lógica de negocio, API RESTful      |
| Frontend (Cliente)    | Next.js, React, TypeScript  | Interfaz de usuario                 |
| Panel de Análisis     | Python, Streamlit, Pandas   | Gestión administrativa, IA          |
| Base de Datos (API)   | Archivos JSON               | Almacenamiento de datos             |
| Backend Independiente | Java, Spring Boot           | Lógica del módulo PI_MOVIL2         |

======================================================================
6. CONCLUSIONES DEL PROYECTO
======================================================================

- La adopción de una **API Central en Node.js** como núcleo facilitó 
  la escalabilidad y flexibilidad.  
- La arquitectura evolucionó de un modelo monolítico a uno modular, 
  permitiendo independencia entre equipos de desarrollo.  
- La definición de contratos claros en la API permitió trabajo en paralelo 
  entre frontend y backend.  
- Aprendimos la importancia de planificar tiempo suficiente para integración 
  y mantener documentación actualizada.  

En conjunto, **Kingdom Barber** entrega una solución moderna, modular y 
funcional, que sienta bases sólidas para futuras expansiones.  

======================================================================

- Escalabilidad:  
  CUMPLE. Arquitectura modular que permite crecimiento del sistema.

======================================================================
