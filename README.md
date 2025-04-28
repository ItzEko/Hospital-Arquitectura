# 🏥 Infraestructura en la nube para un hospital

Repositorio de la infraestructura de servicios en la nube para la gestión hospitalaria.  
Este proyecto está compuesto por microservicios diseñados para ser **desacoplados, escalables y seguros**.

---

## Estructura del Proyecto


---

## Microservicios

### 1. **Microservicio de Autenticación**
- **Responsabilidad**: Manejo de usuarios, login, control de acceso y generación de tokens.
- **Ubicación**: `microservicio-autenticacion/`
- **Tecnologías**: Python, Flask/FastAPI, JWT.

### 2. **Microservicio de Historiales Clínicos**
- **Responsabilidad**: Creación, actualización y consulta de historiales médicos.
- **Ubicación**: `microservicio-historiales/`
- **Tecnologías**: Python, Flask/FastAPI, PostgreSQL.

### 3. **Microservicio de Auditoría**
- **Responsabilidad**: Registro, procesamiento y análisis de eventos del sistema.
- **Ubicación**: `microservicio-auditoria/`
- **Tecnologías**: Python, logging centralizado.

---

## API Gateway

- **Responsabilidad**: Punto único de entrada que enruta solicitudes a los microservicios.
- **Ubicación**: `api-gateway/`
- **Tecnologías**: Python, FastAPI/Flask.

---

## Librerías Compartidas

- **`shared-libs/auth/`**: Funciones comunes de autenticación.
- **`shared-libs/storage/`**: Funciones comunes para gestión de almacenamiento.
- **`shared-libs/monitoring/`**: Funciones comunes de monitoreo.

---

## Instalación Local

### Requisitos Previos
- Python 3.10+
- Docker y Docker Compose
- AWS CLI (opcional para infraestructura)

### Clonación del Repositorio

```bash
git clone https://github.com/tu-usuario/hospital-cloud-infra.git
cd hospital-cloud-infra
