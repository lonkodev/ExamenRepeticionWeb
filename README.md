# Examen de Repetición — CRUD con MySQL
**Asignatura:** IEI-054 Programación Web
**Instituto Profesional Santo Tomás**

---

## Objetivo

Desarrollar un CRUD funcional en Node.js + Express + MySQL, siguiendo la arquitectura MVC vista en clases.

## Contexto

El estudiante elige libremente la entidad sobre la que trabajará el CRUD. Puede reutilizar cualquiera de los ejemplos vistos en clases (estudiantes, productos, libros, etc.) o proponer uno propio. El objetivo es demostrar que recuerda el proceso completo: conexión a base de datos, operaciones CRUD, y separación correcta de responsabilidades.

## Requisitos mínimos

- El proyecto debe ejecutar con `npm start` sin errores.
- Conexión a MySQL funcional (incluir script SQL de la base de datos en el repositorio).
- MVC respetado: **Model = solo estructura**, **Controller = toda la lógica de base de datos** (ningún query fuera del controller).
- Las 4 operaciones (Create, Read, Update, Delete) deben funcionar de extremo a extremo (vista → ruta → controlador → base de datos).
- Repositorio en GitHub con README completo.

## Nulidad automática (nota 1.0)

- Proyecto que no ejecuta.
- Uso de framework CSS (Bootstrap u otro).
- Incumplimiento de formato de entrega.

## Forma de entrega

- Repositorio en GitHub, link enviado al docente. gcaceres6@santotomas.cl
- README con instrucciones de instalación y descripción del proyecto.

---

## Rúbrica de evaluación

| Criterio | 100% | 75% | 60% | 35% | 0% | Ptos |
|---|---|---|---|---|---|---|
| **C — Create** | Formulario y endpoint funcionan, inserta correctamente en BD, valida datos básicos | Inserta correctamente pero sin validación | Inserta pero con errores menores (campos vacíos permitidos, etc.) | Endpoint existe pero no inserta correctamente | No implementado / no funciona | 20 |
| **R — Read** | Lista todos los registros y permite ver detalle individual | Lista todos los registros, sin detalle individual | Lista registros con errores visuales o de datos | Endpoint existe pero no retorna datos correctos | No implementado / no funciona | 20 |
| **U — Update** | Actualiza correctamente, precarga datos existentes en el formulario | Actualiza correctamente sin precarga | Actualiza pero con errores (sobrescribe mal, campos perdidos) | Endpoint existe pero no actualiza | No implementado / no funciona | 20 |
| **D — Delete** | Elimina correctamente y refleja el cambio en la vista | Elimina correctamente sin confirmación | Elimina pero deja inconsistencias (no refresca vista) | Endpoint existe pero no elimina | No implementado / no funciona | 20 |
| **MVC** | Model solo estructura, Controller toda la lógica de BD, sin mezclas | Separación correcta con alguna lógica menor fuera de lugar | Separación parcial (queries en rutas o vistas) | Separación mínima o inconsistente | No hay separación MVC | 10 |
| **GitHub + README** | Repo subido, README completo (instalación, funcionalidades, estructura) | Repo subido, README incompleto | Repo subido, README mínimo | Repo subido sin README | No subido a GitHub | 10 |

**Total: 100 pts → convertidos a escala 1.0–7.0**
