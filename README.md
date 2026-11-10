# Estacionamiento — API REST (Flask)

> **Trabajo académico** · Tecnicatura Universitaria en Programación — UTN, Facultad Regional San Rafael
> **Entrega final del 3.º semestre** (2025) · Equipo **Código Enigma**

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

## Contexto y autoría

Proyecto integrador grupal del equipo **Código Enigma** para la cátedra de
Programación, presentado como entrega final del 3.º semestre. El equipo trabajó
con **rotación de roles**: desarrollo, gestión de tareas y seguimiento de avances
semanales. La subida al repositorio de la cátedra la hacían algunos integrantes
por turno.

Repositorio original de la cátedra:
<https://github.com/PowerSystem2024/CodigoEnigma-ProyectoIntegradorPython>

El README original del equipo se conserva como [`README-original.md`](./README-original.md).
