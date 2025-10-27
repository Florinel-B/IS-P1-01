# IS-P1-01 - Sistema de Monitoreo de Vías Ferroviarias

Primer proyecto de Ingeniería del Software - Grupo 01

## 📋 Descripción del Proyecto

Sistema de monitoreo inteligente para vías ferroviarias que detecta y predice incidencias mediante el análisis de señales eléctricas de dispositivos ubicados en las vías. El sistema permite:

- Lectura de mediciones de voltaje desde archivos CSV
- Detección automática de presencia de trenes en las vías
- Identificación inteligente de incidencias (dispositivos bloqueados, saltos de frecuencia)
- Sistema de suscripciones para notificaciones de incidencias
- Visualización gráfica de datos y incidencias
- API REST para integración con otros sistemas

## 📁 Estructura del Proyecto

```
IS-P1-01/
├── Documentacion_proyecto/
│   ├── IS-P1-2025.md                      # Especificación de la práctica
│   ├── Requisitos_Software.md             # Requisitos funcionales y de dominio
│   ├── Diseño_UML.md                      # Diseño UML completo del sistema
│   ├── Guia_Implementacion_StarUML.md     # Guía paso a paso para StarUML
│   └── Resumen_Diseño_Requisitos.md       # Matriz de trazabilidad y resumen
├── Documentacion_StarUML/                  # Documentación de la herramienta StarUML
├── README.md                               # Este archivo
└── [Carpeta de diagramas UML - pendiente]
```

## 🎯 Requisitos del Sistema

### Requisitos Funcionales
- **R.F.1-5**: Gestión de dispositivos y vías ferroviarias
- **R.F.6**: Detección de presencia de trenes
- **R.F.7**: Módulo inteligente de detección de incidencias
- **R.F.8**: Sistema de suscripciones y notificaciones
- **R.F.9**: Módulo de visualización gráfica

### Requisitos de Dominio
- **R.D.1**: Aplicación web basada en HTTP/REST

Ver detalles completos en: [`Requisitos_Software.md`](Documentacion_proyecto/Requisitos_Software.md)

## 🏗️ Arquitectura del Sistema

El sistema está diseñado con una arquitectura en capas:

1. **Capa de Presentación (REST API)**: Controladores REST para exposición de servicios
2. **Capa de Lógica de Negocio (Services)**: Servicios y módulos inteligentes
3. **Capa de Acceso a Datos (Persistence)**: Repositorios para persistencia

### Paquetes Principales
- **DataAcquisition**: Lectura y gestión de mediciones de sensores
- **IncidentDetection**: Detección y predicción inteligente de incidencias
- **SubscriptionManagement**: Gestión de suscripciones y notificaciones
- **Visualization**: Generación de gráficas y visualizaciones
- **RestAPI**: Endpoints HTTP/REST
- **ServicesLayer**: Lógica de negocio
- **PersistenceLayer**: Acceso a base de datos

## 📐 Diagramas UML

El diseño incluye los siguientes diagramas UML:

1. **Diagrama de Clases**: 30+ clases organizadas en 7 paquetes
2. **Diagrama de Paquetes**: Estructura y dependencias entre módulos
3. **Diagrama de Despliegue**: Infraestructura y nodos de ejecución
4. **Diagrama de Secuencia**: Flujo de detección de incidencias

Ver diseño completo en: [`Diseño_UML.md`](Documentacion_proyecto/Diseño_UML.md)

## 🛠️ Patrones de Diseño Aplicados

- **Strategy**: Para diferentes tipos de incidencias
- **Observer**: Para sistema de notificaciones
- **Repository**: Para abstracción de persistencia
- **DTO**: Para transferencia de datos en la API
- **Facade**: Para simplificar subsistemas complejos

## 🚀 Cómo Empezar

### Para Arquitectos Software

1. Instalar StarUML: https://staruml.io/
2. Leer la guía: [`Guia_Implementacion_StarUML.md`](Documentacion_proyecto/Guia_Implementacion_StarUML.md)
3. Implementar los diagramas siguiendo el diseño: [`Diseño_UML.md`](Documentacion_proyecto/Diseño_UML.md)

### Para Desarrolladores

1. Revisar los requisitos: [`Requisitos_Software.md`](Documentacion_proyecto/Requisitos_Software.md)
2. Estudiar el diseño: [`Diseño_UML.md`](Documentacion_proyecto/Diseño_UML.md)
3. Consultar la matriz de trazabilidad: [`Resumen_Diseño_Requisitos.md`](Documentacion_proyecto/Resumen_Diseño_Requisitos.md)

## 👥 Roles del Equipo

Según la metodología del proyecto:
- **Analistas Software** (2 personas): Captura de requisitos
- **Arquitectos Software** (2 personas): Diseño UML
- **Jefe de Proyectos** (1 persona): Coordinación y metodología ágil

## 📚 Documentación Adicional

- **Especificación del proyecto**: [IS-P1-2025.md](Documentacion_proyecto/IS-P1-2025.md)
- **Manual de StarUML**: [Carpeta Documentacion_StarUML](Documentacion_StarUML/)
- **Resumen ejecutivo**: [Resumen_Diseño_Requisitos.md](Documentacion_proyecto/Resumen_Diseño_Requisitos.md)

## ✅ Estado del Proyecto

- [✓] Captura de requisitos funcionales
- [✓] Captura de requisitos de dominio
- [✓] Diseño de arquitectura del sistema
- [✓] Diagrama de clases completo
- [✓] Diagrama de paquetes
- [✓] Diagrama de despliegue
- [✓] Diagrama de secuencia
- [✓] Documentación de decisiones de diseño
- [✓] Matriz de trazabilidad requisitos-diseño
- [ ] Implementación en StarUML (en progreso)
- [ ] Exportación de diagramas como imágenes
- [ ] Memoria del proyecto

## 📝 Notas de Implementación

### Tecnologías Sugeridas
- **Backend**: Java 17+ con Spring Boot 3.x
- **Frontend**: React/Vue.js con TypeScript
- **Base de Datos**: PostgreSQL 15+
- **Servidor Web**: Nginx o Apache
- **Contenedores**: Docker + Docker Compose

### Principios Aplicados
- ✓ Principios SOLID
- ✓ Separación de responsabilidades
- ✓ Alta cohesión, bajo acoplamiento
- ✓ Diseño orientado a interfaces
- ✓ Extensibilidad y mantenibilidad

## 📅 Calendario

- **Semana 1** (20/10): Análisis y captura de requisitos ✓
- **Semana 2**: Diseño de arquitectura ✓
- **Semanas 3-4**: Refinamiento y documentación (en progreso)
- **Semana 5**: Finalización de documentación
- **Fecha límite**: 20/11 a las 20:00

## 📧 Contacto

Para consultas sobre este proyecto, contactar al jefe de proyecto del grupo.

---

**Universidad Rey Juan Carlos**  
Ingeniería del Software (IS, GIA)  
Curso 2025-2026 
