======================================================================
                💈 PROYECTO INTEGRADOR: KINGDOM BARBER
======================================================================

👥 **Integrantes:**  
- Alejandro Urrego  
- Andrés Vallejo  
- Juan Manuel Rivera  

🏫 **Institución:**  
Institución Técnica CESDE  

📆 **Fecha:**  
Octubre, 2025  

======================================================================
             📺 VISOR INTERACTIVO DE DOCUMENTACIÓN
======================================================================

Este repositorio incluye un archivo `index.html` que actúa como una **presentación interactiva** de toda la documentación del proyecto.

### ▶️ Cómo Ejecutarlo:
1. Haz doble clic en el archivo `index.html`, **o**  
2. Arrástralo a una pestaña nueva de tu navegador.  

No requiere ningún servidor ni comandos adicionales.

======================================================================
             💈 KINGDOM BARBER - ECOSISTEMA INTEGRAL
======================================================================

¡Bienvenido al repositorio central de **Kingdom Barber**!  
Aquí comprenderás la **arquitectura completa** del ecosistema que moderniza la gestión de barberías a través de tecnología, análisis e inteligencia artificial.

======================================================================
                 📜 1. VISIÓN GENERAL DEL PROYECTO
======================================================================

**Kingdom Barber** es un **ecosistema de software completo y desacoplado**, diseñado para modernizar la gestión de barberías.

El sistema está compuesto por **tres proyectos independientes pero conectados**, que funcionan en sinergia:

| Componente | Descripción |
|-------------|-------------|
| 🧠 **API Central (Back-End)** | Desarrollada en Java con Spring Boot. Es el cerebro del sistema, maneja la lógica de negocio y los datos. |
| 🌐 **Plataforma Web (Front-End)** | Construida con Next.js (React), permite la interacción con clientes y barberos (agendamiento, galería, contacto). |
| 📊 **Panel de Gestión (Análisis)** | Desarrollado en Python con Streamlit, ofrece dashboards, KPIs y un asistente de IA para análisis e informes. |

======================================================================
                    🏗️ 2. ARQUITECTURA DEL SISTEMA
======================================================================

El sistema sigue una **arquitectura de servicios desacoplados**, donde la **API de Java** actúa como **única fuente de verdad**.  
Los dos clientes front-end (Next.js y Streamlit) consumen sus endpoints vía HTTP.

```
┌───────────────────────────────┐
│         API CENTRAL           │
│  Java + Spring Boot (8080)    │
│  └── Lógica de negocio y BD   │
└────────────┬──────────────────┘
             │
 ┌───────────┼────────────┐
 │                        │
 ▼                        ▼
🌐 Plataforma Web     📊 Panel de Gestión
Next.js / React       Streamlit / Python
Puerto 3000           Puerto 8501
```

======================================================================
                🚀 3. REPOSITORIOS DEL ECOSISTEMA
======================================================================

| Proyecto | Tecnología | Repositorio | Descripción |
|-----------|-------------|-------------|--------------|
| 🧠 **API Central (pi_movil2.0)** | Java + Spring Boot | [🔗 GitHub](https://github.com/JuanRivera24/pi_movil2.0.git) | Lógica de negocio, controladores, modelos y base de datos. |
| 🌐 **Plataforma Web (pi_web2.0)** | Next.js + React + TS | [🔗 GitHub](https://github.com/JuanRivera24/pi_web2.0.git) | Interfaz de usuario para clientes y barberos. |
| 📊 **Panel de Gestión (pi_ntp2.0)** | Python + Streamlit | [🔗 GitHub](https://github.com/JuanRivera24/pi_ntp2.0.git) | Dashboard de análisis, KPIs y Asistente de IA. |

======================================================================
             ⚙️ 4. CÓMO EJECUTAR EL ECOSISTEMA COMPLETO
======================================================================

Para usar el sistema completo, **ejecuta los tres proyectos** en el siguiente orden:

#### 1️⃣ Iniciar la API Central (Java)
```
cd pi_movil2
./mvnw spring-boot:run
```
API disponible en 👉 `http://localhost:8080`

#### 2️⃣ Iniciar el Panel de Gestión (Python)
```
cd pi_ntp
.venv\Scripts\activate
streamlit run inicio.py
```
Panel disponible en 👉 `http://localhost:8501`

#### 3️⃣ Iniciar la Plataforma Web (Next.js)
```
cd pi_web2
npm run dev
```
Web disponible en 👉 `http://localhost:3000`

✅ Una vez los tres servicios estén activos, el ecosistema estará completamente funcional.

======================================================================
                🧭 5. INTRODUCCIÓN Y VISIÓN GENERAL
======================================================================

### 5.1. Resumen del Proyecto
**Kingdom Barber** representa la evolución hacia una **plataforma digital integral** para la gestión de barberías.  
Su objetivo es ofrecer una solución robusta que optimice la administración, fortalezca la relación con el cliente y brinde herramientas de análisis inteligentes.

El ecosistema integra:
- 🧠 **API Central:** Java + Spring Boot  
- 🌐 **Plataforma Web:** Next.js + React  
- 📊 **Panel de Gestión:** Python + Streamlit  

### 5.2. Planteamiento del Problema
Las barberías aún dependen de métodos manuales, carecen de sistemas integrados y no explotan los datos de forma inteligente, generando:
- Ineficiencia en la gestión de citas.  
- Falta de análisis estratégico.  
- Experiencia limitada para el cliente moderno.

### 5.3. Solución Propuesta
- Digitalizar procesos clave (reservas, gestión, reportes).  
- Centralizar la lógica en una API robusta (Java).  
- Ofrecer interfaces modernas, rápidas y seguras.  
- Incluir inteligencia artificial para análisis y decisiones.

======================================================================
                   🎯 6. OBJETIVOS DEL PROYECTO
======================================================================

### 🎯 Objetivo General
Desarrollar un **ecosistema de software integral y escalable** que modernice la gestión de barberías y potencie la toma de decisiones basadas en datos.

### 🔹 Objetivos Específicos
- 🧩 **Centralizar Lógica:** API REST en Java como fuente única de verdad.  
- 💻 **Experiencia Moderna:** Web en Next.js para clientes y barberos.  
- 📊 **Gestión con Datos:** Dashboard Streamlit con métricas e IA.  
- 🤖 **Asistente de IA:** Análisis en lenguaje natural (Gemini).  
- ⚙️ **Escalabilidad:** Arquitectura modular y desacoplada.

======================================================================
                🧱 7. MÓDULOS DEL PROYECTO
======================================================================

### 🔹 Módulo 1: API Central (Java + Spring Boot)
- CRUD completo de entidades: citas, usuarios, servicios, sedes.  
- Subida y almacenamiento de imágenes en Base64.  
- Configuración CORS para comunicación segura.  
- Lógica enriquecida de datos (nombre sede, barbero, etc.).

### 🔹 Módulo 2: Plataforma Web (Next.js + React)
- Autenticación de usuarios con Clerk.  
- Calendario de citas en tiempo real.  
- Galería, contacto y agenda personal del barbero.  
- 100% responsiva y conectada a la API.

### 🔹 Módulo 3: Panel de Gestión (Python + Streamlit)
- Dashboard con KPIs y gráficos interactivos.  
- Filtros avanzados para citas e ingresos.  
- Exportación de datos e informes PDF.  
- Asistente de IA (Gemini) para análisis estratégico.

======================================================================
              🧠 8. STACK TECNOLÓGICO CONSOLIDADO
======================================================================

| Capa | Tecnología | Propósito |
|------|-------------|-----------|
| ⚙️ Back-End | Java, Spring Boot, JPA, H2 | Lógica y persistencia de datos |
| 🌐 Front-End | Next.js, React, TypeScript, Tailwind | Interfaz cliente y barbero |
| 📊 Análisis | Python, Streamlit, Pandas, Plotly | BI, reportes, IA integrada |

======================================================================
        🧩 9. DIFICULTADES Y LECCIONES APRENDIDAS
======================================================================

### 🔸 Desafíos Técnicos
- **CORS y comunicación multi-origen:** ajustes detallados en Spring Boot.  
- **Inconsistencias de nomenclatura:** se solucionó con una capa de traducción en `data_manager.py`.  
- **Migración de archivos a base de datos relacional:** rediseño de entidades.  
- **Gestión de imágenes Base64:** solución robusta frente a rutas locales.  
- **“Contrato de API” estable:** coordinación constante entre equipos.

### 🔸 Lecciones Aprendidas
- Importancia del desac acoplamiento total entre capas.  
- Necesidad de definir estándares desde el inicio (nombres, rutas, JSONs).  
- Ventajas de trabajar con una API única para varios clientes.  
- Valor del trabajo colaborativo y la integración continua.

======================================================================
                   🏁 10. CONCLUSIONES FINALES
======================================================================

- ✅ **Evolución tecnológica:** de un sistema híbrido a una arquitectura moderna y limpia.  
- 🧠 **Consistencia:** la API central garantiza integridad y escalabilidad.  
- 💪 **Logro técnico:** integración exitosa de tres stacks distintos (Java, Python, JavaScript).  
- 🚀 **Base sólida:** lista para futuras expansiones (ej. app móvil).  

El proyecto **Kingdom Barber** consolida un ecosistema tecnológico moderno, cohesivo y profesional, que demuestra dominio en **arquitecturas desacopladas, integración de tecnologías y análisis inteligente de datos**.

======================================================================
                     ✨ FIN DEL DOCUMENTO
======================================================================

