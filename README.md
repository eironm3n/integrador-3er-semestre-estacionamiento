# Estacionamiento — API REST (Flask)

> **Continuación individual de un proyecto académico** · Base: proyecto integrador del 3.º semestre
> de la Tecnicatura Universitaria en Programación — UTN, Facultad Regional San Rafael (2025),
> realizado con el equipo **Código Enigma**. Ver [Origen del proyecto](#origen-del-proyecto).

Aplicación web para gestionar el cobro de un estacionamiento según el tiempo de
permanencia del vehículo: registro de ingreso y egreso, cálculo automático del
monto a pagar, temporizador y verificación del estado del servidor en tiempo
real. Documentación de la API navegable con Swagger UI.

## Tecnologías

- **Python 3** · **Flask** — API REST
- **SQLAlchemy** sobre **SQLite** — persistencia (`app/patentes.db`)
- **Flask-RESTX** + **Swagger UI** — documentación de endpoints (`/docs`)
- Arquitectura en capas por módulo: `controllers` / `models` / `repositories` / `services`
- Carga dinámica de controladores y registro dinámico de *namespaces*
- Frontend responsive en HTML / CSS / JavaScript

## Ejecución

```bash
python -m venv env
# Windows: .\env\Scripts\activate   |   Linux/macOS: source env/bin/activate
pip install -r requirements.txt
python run.py
```

API en `http://127.0.0.1:5000/home` · documentación en `http://127.0.0.1:5000/docs`.

## Origen del proyecto

Este repositorio toma como **base el proyecto integrador de la Tecnicatura
Universitaria en Programación** (UTN, Facultad Regional San Rafael) para la
cátedra de Programación. El proyecto se comenzó en **mayo de 2025** y se realizó
durante el 3.º semestre con el equipo **Código Enigma**, hasta su entrega final
en **junio de 2025**.

Durante la tecnicatura el equipo trabajó con **rotación de roles** (desarrollo,
gestión de tareas y seguimiento de avances semanales), y la subida al repositorio
de la cátedra la hacían algunos integrantes por turno.

### Continuación individual

A partir de esa base, **Arón Rojas**, integrante del equipo, continúa el proyecto
de forma individual en este repositorio:

- Actualización de dependencias (Flask, Werkzeug, flask-cors y el resto): sin
  vulnerabilidades conocidas, verificado con las mismas respuestas de la API que antes.
- Documentación técnica corregida (persistencia con SQLAlchemy sobre SQLite y Flask-RESTX).

### Repositorio original de la cátedra

<https://github.com/PowerSystem2024/CodigoEnigma-ProyectoIntegradorPython>

El README original del equipo se conserva como [`README-original.md`](./README-original.md).
