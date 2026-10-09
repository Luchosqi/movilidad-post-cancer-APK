# Movilidad Post-Cáncer

App Android **para pacientes** sobrevivientes de cáncer. El profesional encargado asigna ejercicios desde la web; el paciente los realiza siguiendo la guía de la app. La cámara del teléfono detecta sus movimientos durante la ejecución y la app registra mediciones de cada sesión para que el profesional pueda revisar su evolución.

## Problemática

Los tratamientos oncológicos (quimioterapia, radioterapia) pueden generar secuelas
motoras que reducen el rango de movimiento en hombros, codos, cadera y columna, entre
otras articulaciones. Muchas veces estas limitaciones no se detectan ni se cuantifican
de forma sistemática, lo que dificulta un seguimiento oportuno de la rehabilitación del
paciente.

Este proyecto busca apoyar la realización y medición de ejercicios de movilidad asignados por el profesional, para que pueda seguir la evolución de cada paciente. Es una herramienta de **apoyo**, no de diagnóstico clínico.

## Objetivo general

Desarrollar un sistema en el que el profesional encargado asigne ejercicios de movilidad, el paciente los realice con guía y detección de movimientos por la cámara del teléfono, y el profesional consulte los resultados y la evolución en un dashboard por paciente.

## Objetivos específicos

1. Diseñar un protocolo digital de ejercicios de movilidad asignados por el profesional y guiados en la app del paciente.
2. Implementar en web la asignación de ejercicios y un dashboard por paciente para registrar y comparar sesiones a lo largo del tiempo.
3. Detectar movimientos con la cámara del teléfono y definir indicadores objetivos (ángulos, tiempos, repeticiones y calidad de medición).
4. Validar el protocolo y las mediciones con profesionales de la salud para asegurar su pertinencia clínica.

## Equipo — Iteración 1

| Integrante | Rol en esta iteración |
| --- | --- |
| **Emilia Toro** (coordinadora) | Coordinación general del equipo, elaboración de la guía de entrevista y gestión del contacto con la contraparte, y liderazgo de la validación clínica con profesionales de la salud (objetivo específico 4). |
| **Luis Jaramillo** | Investigación y desarrollo del protocolo de ejercicios guiados para la app del paciente (objetivo específico 1), detección de movimientos con la cámara e indicadores de medición (objetivo específico 3). |
| **Cristian Sandoval** | Investigación y desarrollo de la asignación de ejercicios, el dashboard individual y la comparación de mediciones a lo largo del tiempo en web (objetivo específico 2). |

### Rotación de coordinación

- Iteración 1: Emilia Toro
- Iteración 2: Luis Jaramillo
- Iteración 3: Cristian Sandoval

A partir de la cuarta iteración (si el semestre lo requiere), la rotación se reinicia en
el mismo orden.

## Convención de trabajo

Ambos repositorios siguen el [mismo GitFlow y la convención de commits atómicos](CONTRIBUTING.md): `main` contiene entregas estables, `develop` integra el siguiente avance y cada tarea se desarrolla en `feature/*`. Las ramas `release/*` y `hotfix/*` se usan al preparar entregas o corregirlas. Los commits siguen Conventional Commits; la revisión por otro integrante precede a la integración, sin exigir un PR.

## Contexto

Proyecto del curso **Comprensión del Contexto Social 2026**.

## Trabajo entre APK y web

Este repositorio desarrolla la app del paciente: consulta los ejercicios asignados, guía su ejecución, detecta movimientos mediante la cámara del teléfono y envía las sesiones medidas. El repositorio [web](https://github.com/Luchosqi/movilidad-post-cancer-web) es para el profesional encargado: asigna ejercicios y consulta el dashboard individual, historial y evolución de cada paciente. Tras acordar el stack, web también mantendrá la API y persistencia compartida. La división, etapas, responsables iniciales y decisiones pendientes están en el [plan de trabajo compartido](https://github.com/Luchosqi/movilidad-post-cancer-web/blob/main/docs/plan-de-trabajo.md). Los formatos de asignación y sesión se proponen en el [contrato de web](https://github.com/Luchosqi/movilidad-post-cancer-web/blob/main/docs/contrato-integracion.md).

Por ahora ambos repositorios documentan el alcance; todavía no hay una aplicación implementada. Los ejemplos de integración usan datos sintéticos.

## Especificación y prototipo

La [especificación de requerimientos compartida](https://github.com/Luchosqi/movilidad-post-cancer-web/blob/main/docs/Especificacion_de_requerimientos_Movilidad_Post_Cancer.docx) define los requisitos verificables de la app del paciente, la web del profesional y su integración. El [prompt móvil para Figma Make](https://github.com/Luchosqi/movilidad-post-cancer-web/blob/main/docs/prompts-figma-make.md#prompt-1-app-android-del-paciente) describe las pantallas M01–M06 y sus estados para el prototipo de alta fidelidad. Los ejercicios y datos de demostración requieren validación clínica antes de usarse con pacientes reales.
