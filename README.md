======================================================================
                 KINGDOM BARBER - SISTEMA DE GESTIÓN
======================================================================

📖 DESCRIPCIÓN GENERAL
----------------------

Kingdom Barber es una plataforma integral que busca digitalizar y optimizar
la gestión de barberías.  

El ecosistema está compuesto por tres módulos principales:

- **PI_WEB2 (Frontend Cliente/Barbero)**:  
  Desarrollado en Next.js (React + Tailwind), ofrece la interfaz para 
  clientes y barberos.

- **PI_MOVIL2 (Backend / API REST)**:  
  Construido con Spring Boot en Java, maneja la lógica de negocio, 
  seguridad y persistencia de datos.

- **PI_NTP (Panel de Gestión / Dashboard con IA)**:  
  Aplicación desarrollada en Python con Streamlit, diseñada para la 
  administración avanzada, análisis de métricas y generación de reportes 
  mediante Inteligencia Artificial.

======================================================================
                   ✨ CARACTERÍSTICAS PRINCIPALES
======================================================================

-----------------------------
-- PORTAL DEL CLIENTE (PI_WEB2) --
-----------------------------

- Reservar Cita:
  Formulario intuitivo para seleccionar sede, barbero, servicio y horario.

- Visualizar Barberos:
  Listado dinámico con información de barberos disponibles por sede.

- Gestión de Citas:
  Posibilidad de modificar o cancelar reservas existentes.

-----------------------------
-- PORTAL DEL BARBERO (PI_WEB2) --
-----------------------------

- Inicio de Sesión por Sede:
  Selección de sede y nombre para acceder a la agenda personal.

- Visualización de Agenda:
  Listado con citas agendadas (fecha, hora, cliente, servicio).

- Detalles de la Cita:
  Página dedicada con toda la información del servicio y cliente.

- Cancelación de Citas:
  Opción para anular citas desde la propia agenda.

-----------------------------
-- PANEL DE GESTIÓN (PI_NTP) --
-----------------------------

- Dashboard General:
  KPIs de ingresos, citas, servicios y barberos top.

- Filtros Avanzados:
  Por sede, barbero, cliente y rango de fechas.

- Gráficos Interactivos:
  Distribución de ingresos, carga de trabajo y evolución de citas.

- Asistente IA:
  Generador de reportes, analista de datos, marketing inteligente, 
  detección de oportunidades y asesor de estilo virtual.

======================================================================
               🛠️ TECNOLOGÍAS Y ARQUITECTURA
======================================================================

-----------------------------
-- BACKEND (PI_MOVIL2 - SPRING BOOT) --
-----------------------------

- Lenguaje: Java
- Framework: Spring Boot
- Arquitectura: MVC + API REST
- Persistencia: Spring Data JPA + SQL

**Componentes Clave:**
- Controladores: Endpoints RESTful para CRUD de citas, barberos, clientes.
- Modelos: Entidades JPA que representan la base de datos.
- Repositorios: Interfaces para operaciones CRUD automáticas.

-----------------------------
-- FRONTEND (PI_WEB2 - NEXT.JS) --
-----------------------------

- Lenguajes: TypeScript, JavaScript (ES6+), HTML5, CSS3
- Framework: Next.js + React
- Estilos: Tailwind CSS

**Características Clave:**
- Rutas dinámicas y componentes reutilizables.
- Peticiones a la API con fetch/axios.
- Diseño responsivo y moderno.
- Separación de vistas por roles (cliente/barbero).

-----------------------------
-- PANEL DE GESTIÓN (PI_NTP - STREAMLIT) --
-----------------------------

- Lenguaje: Python
- Framework: Streamlit
- Librerías: Pandas, Plotly, ReportLab
- IA: Análisis de datos y generación de reportes automáticos

======================================================================
        ✅ CUMPLIMIENTO DE REQUISITOS DEL PROYECTO
======================================================================

-----------------------------
-- FRONTEND --
-----------------------------

- Formularios de Ingreso (inputs, submit en HTML):  
  CUMPLE. Formularios claros para agendar citas y seleccionar sede/barbero.

- Captura de Datos con JSON:  
  CUMPLE. Se envían y reciben datos en formato JSON.

- Peticiones con fetch/axios:  
  CUMPLE. Implementadas para GET, POST, PUT y DELETE.

- Presentación Mejorada:  
  CUMPLE. Interfaz moderna con Tailwind, responsiva y estructurada.

-----------------------------
-- BACKEND --
-----------------------------

- Endpoints REST:  
  CUMPLE. Controladores con operaciones CRUD para citas, barberos y clientes.

- Procesamiento de Datos:  
  CUMPLE. Incluye lógica de negocio (ej. validación de clientes al crear cita).

- Conexión a BD:  
  CUMPLE. Persistencia con JPA y base SQL.

- Respuestas en JSON:  
  CUMPLE. Respuestas automáticas procesadas por Spring Boot.

-----------------------------
-- PANEL DE GESTIÓN --
-----------------------------

- Dashboard Interactivo:  
  CUMPLE. Visualización de KPIs con gráficos dinámicos.

- Filtros Avanzados:  
  CUMPLE. Aplicados en tiempo real sobre datos históricos.

- Reportes en PDF:  
  CUMPLE. Generación automática con análisis interpretativo.

- IA Integrada:  
  CUMPLE. Asistente con submódulos especializados para análisis y marketing.

-----------------------------
-- REQUISITOS ADICIONALES --
-----------------------------

- Roles Diferenciados:  
  CUMPLE. Cliente y Barbero con accesos y vistas específicas.

- Experiencia de Usuario:  
  CUMPLE. Flujo intuitivo y diseño atractivo.

- Escalabilidad:  
  CUMPLE. Arquitectura modular que permite crecimiento del sistema.

======================================================================
