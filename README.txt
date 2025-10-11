


======================================================================
             💈 PROYECTO INTEGRADOR: KINGDOM BARBER
======================================================================

👥 Integrantes:  
Alejandro Urrego  
Andrés Vallejo  
Juan Manuel Rivera  

🏫 Institución: Institución Técnica CESDE  
📆 Fecha: Octubre, 2025  

======================================================================
                  📺 VISOR INTERACTIVO DE DOCUMENTACIÓN
======================================================================

Este repositorio incluye un archivo `index.html` que funciona como una
presentación interactiva de toda la documentación del proyecto.  

Para visualizarlo, simplemente abre el archivo en tu navegador.

======================================================================
                   📖 1. VISIÓN GENERAL DEL PROYECTO
======================================================================

Kingdom Barber es un ecosistema de software completo y desacoplado,
diseñado para modernizar la gestión de barberías y optimizar la
experiencia de clientes, barberos y administradores.

Su objetivo principal es ofrecer una plataforma robusta que integre
tres aplicaciones conectadas, desplegadas de manera independiente pero
sincronizadas mediante una API central:

Componente | Descripción
----------- | -------------
🧠 **API Central (Back-End)** | Desarrollada en **Java + Spring Boot**, maneja la lógica de negocio y la persistencia.
🌐 **Plataforma Web (Front-End)** | Construida con **Next.js (React)**, permite a clientes y barberos agendar, visualizar y gestionar citas.
📊 **Panel de Gestión (Análisis)** | Creado con **Python + Streamlit**, ofrece dashboards, KPIs y un Asistente de IA para análisis y reportes.

======================================================================
                🏗️ 2. ARQUITECTURA Y APLICACIONES DESPLEGADAS
======================================================================

El ecosistema sigue una **arquitectura de servicios desacoplados**, donde
la **API Central** actúa como la **única fuente de verdad** para los
módulos de análisis y front-end.

                        ┌──────────────────────────────┐
                        │     API CENTRAL (Back-End)    │
                        │     Java + Spring Boot        │
                        │     [Render]                  │
                        └──────────────┬───────────────┘
                                       │
                     (Peticiones HTTP / JSON)
                                       │
      ┌────────────────────────────┬────────────────────────────┐
      │                            │                            │
      ▼                            ▼                            ▼
┌──────────────────────┐     ┌──────────────────────────┐
│ PLATAFORMA WEB       │     │ PANEL DE GESTIÓN (IA)    │
│ Next.js + React       │     │ Python + Streamlit       │
│ [Vercel]              │     │ [Streamlit Cloud]        │
└──────────────────────┘     └──────────────────────────┘

🚀 **Aplicaciones en Producción**
----------------------------------------------------------------------
🌐 Plataforma Web → https://pi-web2-six.vercel.app  
📊 Panel de Gestión → https://kingdombarberdashboard.streamlit.app  
🧠 API Central (Test) → https://pi-movil2-0.onrender.com/sedes  

======================================================================
                   🚀 3. REPOSITORIOS DEL ECOSISTEMA
======================================================================

Proyecto | Tecnología | Repositorio
----------|-------------|-------------
🧠 **API Central (pi_movil2)** | Java + Spring Boot | 🔗 [Ver en GitHub](https://github.com/JuanRivera24/pi_movil2.0)
🌐 **Plataforma Web (pi_web2)** | Next.js + React + TypeScript | 🔗 [Ver en GitHub](https://github.com/JuanRivera24/pi_web2)
📊 **Panel de Gestión (pi_ntp)** | Python + Streamlit | 🔗 [Ver en GitHub](https://github.com/JuanRivera24/pi_ntp)

======================================================================
             ⚙️ 4. CÓMO EJECUTAR EL ECOSISTEMA LOCALMENTE
======================================================================

Para ejecutar todo el ecosistema de Kingdom Barber localmente:

1️⃣ **Iniciar la API Central (Java)**  
--------------------------------------------------
cd pi_movil2  
./mvnw spring-boot:run  
Disponible en 👉 http://localhost:8080  

2️⃣ **Iniciar el Panel de Gestión (Python)**  
--------------------------------------------------
cd pi_ntp  
.venv\Scripts\activate  
streamlit run inicio.py  
Disponible en 👉 http://localhost:8501  

3️⃣ **Iniciar la Plataforma Web (Next.js)**  
--------------------------------------------------
cd pi_web2  
npm run dev  
Disponible en 👉 http://localhost:3000  

======================================================================
                      🎯 5. OBJETIVOS DEL PROYECTO
======================================================================

🎯 **Objetivo General:**  
Desarrollar un ecosistema de software integral y escalable que
modernice la gestión de barberías, mejore la experiencia del cliente y
potencie la toma de decisiones con datos.

🔹 **Objetivos Específicos:**  
- 🧩 **Centralizar Lógica:** Implementar una API REST como fuente de verdad.  
- 💻 **Experiencia Moderna:** Crear un front-end en Next.js para clientes y barberos.  
- 📊 **Gestión con Datos:** Diseñar un dashboard analítico en Streamlit.  
- 🤖 **Integrar IA:** Incluir un asistente Gemini para análisis inteligente.  
- 📈 **Análisis de Mercado:** Conectar datasets públicos para estudios estadísticos.  

======================================================================
                🧱 6. STACK TECNOLÓGICO CONSOLIDADO
======================================================================

Capa | Tecnología | Propósito
------|-------------|-------------
⚙️ **Back-End (API)** | Java, Spring Boot, Spring Data JPA, PostgreSQL | Lógica de negocio y persistencia de datos.  
🌐 **Front-End (Cliente)** | Next.js, React, TypeScript, Tailwind CSS, Clerk | Interfaz para usuarios y barberos.  
📊 **Análisis de Datos** | Python, Streamlit, Pandas, Plotly, Gemini | Reportes, BI y asistente de IA.  

======================================================================
           🧩 7. DIFICULTADES Y LECCIONES APRENDIDAS
======================================================================

🔧 **Integración Multi-Tecnológica:**  
El principal reto fue sincronizar la comunicación entre Java, Python y
JavaScript. Se resolvieron problemas de CORS y se estableció un formato
de datos unificado.

🧹 **Calidad de Código y Linters:**  
Las plataformas de despliegue forzaron a depurar importaciones, hooks y
dependencias, lo que mejoró la calidad general del código.

🖼️ **Gestión de Imágenes:**  
El almacenamiento en Base64 dentro de la base de datos resolvió los
problemas de rutas y CORS, resultando en una solución segura y limpia.

🤝 **Contrato de API:**  
Se aprendió la importancia de mantener un contrato de API estable, ya
que cualquier cambio en el back-end afecta directamente los front-ends.

======================================================================
                     🏁 8. CONCLUSIONES FINALES
======================================================================

✅ **Evolución Tecnológica:**  
Se migró de un sistema fragmentado a una arquitectura moderna y limpia.

💪 **Logro Técnico:**  
Se integraron con éxito tres stacks tecnológicos distintos en un solo
ecosistema funcional.

🚀 **Base Escalable:**  
El sistema está preparado para futuras ampliaciones, como una app móvil
nativa o integración con nuevos servicios.

El proyecto **Kingdom Barber** representa la consolidación de un
ecosistema profesional, modular y moderno, enfocado en calidad,
escalabilidad y experiencia del usuario.

======================================================================
                           ✨ FIN DEL DOCUMENTO
======================================================================
