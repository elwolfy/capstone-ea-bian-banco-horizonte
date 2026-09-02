# Capstone — Arquitectura Bancaria con BIAN · Banco Horizonte

Proyecto integrador del curso **CD-03 · Arquitectura Bancaria basada en el Estándar BIAN® (v14)** — CPS Tech.
Repositorio del **proyecto ArchiMate** del Capstone, que se **actualiza en cada sesión**.

> **Aviso:** «Banco Horizonte» es una entidad **ficticia** con fines didácticos.

## ¿Qué contiene este repositorio?

- **El caso de negocio** (insumo, en lenguaje de negocio): misión, modelo de negocio, marco regulatorio, funciones, procesos y assessment de co-creación.
- **El modelo ArchiMate** del Capstone (gestionado con el plugin **coArchi**), donde sesión a sesión se construyen las vistas de arquitectura.

## Estructura de carpetas

```
/
├─ README.md
├─ docs/
│  └─ Caso-de-Negocio-Banco-Horizonte.md      # el caso (insumo)
├─ model/                                       # modelo ArchiMate (lo crea/gestiona coArchi)
└─ assets/                                       # imágenes, exportaciones (opcional)
```

## Herramientas

| Herramienta | Uso |
|---|---|
| **Archi** | Modelado en ArchiMate 3.2 |
| **jArchi** | Scripts (JScript) para generar vistas de forma automatizada |
| **coArchi** | Colaboración y versionado del modelo contra este repositorio Git |
| **GitHub** | Repositorio remoto del proyecto |

## Flujo de trabajo por sesión

1. **Pull** del repositorio (traer los últimos cambios) desde la vista *Collaboration* de Archi.
2. Trabajar la(s) vista(s) de la sesión (manual o con scripts jArchi).
3. **Commit** con un mensaje claro (p. ej. `M1: vista motivacional y de capacidades`).
4. **Push** al repositorio.

## Vistas por módulo (assignments)

| Módulo | Vista(s) a construir |
|---|---|
| **1** | Vista **motivacional**, vista de **capacidades** y vista **estratégica** |
| **2** | Vistas de **procesos y procedimientos** (nivel de actividades) y **core actual** |
| **3–4** | Superposición de **Service Domains** de BIAN |
| **5–6** | Arquitectura de **datos / BOM** |
| **7–8** | Solución **TO-BE** (microservicios y APIs) |
| **9–10** | **Roadmap** de arquitectura y migración |
