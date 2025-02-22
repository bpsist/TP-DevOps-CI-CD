# TP-DevOps 2024

## Requisitos

- **Python 3.x**
- **Cliente MySQL** (Ejemplo: [Dbeaver](https://dbeaver.io/download/))
- **Docker** y **Docker Compose**
- **Node.js**
- **REACT**

## Objetivo

Aplicar los conocimientos adquiridos en la materia _Desarrollo y Operaciones_ para mejorar el CI/CD del proyecto dado, compuesto por 3 microservicios utilizando un proxy para que tanto el frontend como el backend salgan por el mismo dominio.

### Objetivos Específicos

- Automatizar los procesos de build y deploy de los microservicios dados para mejorar la entrega continua.
- Automatizar el análisis de SAST del producto, mitigando las vulnerabilidades actuales conocidas y teniendo en cuenta las buenas prácticas.
- Proponer mejoras al trabajo entregado.
- Documentar errores y soluciones aplicadas.

## Puntos de Entrega

### 1. Pipeline en el Repositorio

- **No debe haber secretos hardcodeados** en los archivos del repositorio.

#### 1.1 Seguridad en el Repositorio

- Escaneo de **Secretos** para cada microservicio.

#### 1.2 Escaneo/Linting de Código

- Para cada microservicio (excepción: base de datos).
- **Debe generar artefactos**.

#### 1.3 Build

- 1 Base de datos.
- 2 APIs en distintos lenguajes expuestos por medio de NGINX:
  - **Python**
  - **Node.js**
- 1 Frontend en NGINX: **REACT**.
- **Push al Registry del LabSis**.

#### 1.4 Escaneo/Linting de Docker

- Estático y Linting para cada microservicio.
- **Debe generar artefactos**.

#### 1.5 Deploy

- Usando **SSH**.
- Mostrar que los **containers están corriendo**.

---

### 2. Bitácora de Pipeline Ejecutado

En un archivo `pipeline.md` en el repositorio, adjuntar:

- **Imágenes de un pipeline exitoso** e imágenes de cada uno de los jobs.
- **Linkeado a esta sección**.
- Las imágenes deben colocarse en una carpeta `imgs` en la raíz del repositorio.

---

### 3. Verificación de Deploy

En un archivo `health-checks.md` en el repositorio, linkeado a esta sección:

- Este archivo debe contener información sobre **cómo verificar cada servicio deployado**.

---

### 4. Glosario de Errores

En un archivo `errores.md` en el repositorio, linkeado a esta sección:

- Errores que enfrentaron: identificación de error y cómo lo solucionaron.

---

### 5. Conclusiones

En un archivo `conclusiones.md` en el repositorio, linkeado a esta sección:

- Posibles mejoras al pipeline.
- Puntos de mejora.

---
