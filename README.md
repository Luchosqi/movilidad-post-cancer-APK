# Movilidad Post-Cáncer

Sistema para evaluar el estado inicial de movilidad de pacientes sobrevivientes de
cáncer, identificando limitaciones en el rango de movimiento mediante ejercicios
guiados.

## Problemática

Los tratamientos oncológicos (quimioterapia, radioterapia) pueden generar secuelas
motoras que reducen el rango de movimiento en hombros, codos, cadera y columna, entre
otras articulaciones. Muchas veces estas limitaciones no se detectan ni se cuantifican
de forma sistemática, lo que dificulta un seguimiento oportuno de la rehabilitación del
paciente.

Este proyecto busca ofrecer una evaluación objetiva y accesible del rango de movimiento
que permita detectar posibles limitaciones y hacer seguimiento de su evolución. Es una
herramienta de **apoyo**, no de diagnóstico clínico.

## Objetivo general

Desarrollar un sistema que permita evaluar el estado inicial de movilidad de pacientes
sobrevivientes de cáncer, identificando limitaciones en el rango de movimiento mediante
ejercicios guiados.

## Objetivos específicos

1. Diseñar un protocolo digital de ejercicios de evaluación para medir el rango de
   movimiento en articulaciones frecuentemente afectadas por tratamientos oncológicos.
2. Implementar un módulo de registro y visualización del estado inicial del paciente
   que permita comparar mediciones a lo largo del tiempo.
3. Definir indicadores objetivos (ángulos, tiempos, repeticiones) que faciliten la
   detección temprana de problemas de movilidad.
4. Validar la propuesta con profesionales de la salud para asegurar la pertinencia
   clínica de las mediciones obtenidas.

## Equipo — Iteración 1

| Integrante | Rol en esta iteración |
| --- | --- |
| **Emilia Toro** (coordinadora) | Coordinación general del equipo, elaboración de la guía de entrevista y gestión del contacto con la contraparte, y liderazgo de la validación clínica con profesionales de la salud (objetivo específico 4). |
| **Luis Jaramillo** | Investigación y desarrollo del protocolo digital de ejercicios de evaluación del rango de movimiento (objetivo específico 1) y definición de los indicadores objetivos de medición —ángulos, tiempos, repeticiones— (objetivo específico 3). |
| **Cristian Sandoval** | Investigación y desarrollo del módulo de registro y visualización del estado inicial del paciente, incluyendo la lógica para comparar mediciones a lo largo del tiempo (objetivo específico 2). |

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

Este repositorio desarrolla la experiencia Android del paciente y la medición local. El repositorio [web](https://github.com/Luchosqi/movilidad-post-cancer-web) desarrollará la vista para profesionales y, tras acordar el stack, la API y persistencia compartida. La división, etapas, responsables iniciales y decisiones pendientes están en el [plan de trabajo compartido](https://github.com/Luchosqi/movilidad-post-cancer-web/blob/main/docs/plan-de-trabajo.md). El formato de sesión se propone en el [contrato de web](https://github.com/Luchosqi/movilidad-post-cancer-web/blob/main/docs/contrato-integracion.md).

Por ahora ambos repositorios documentan el alcance; todavía no hay una aplicación implementada. Los ejemplos de integración usan datos sintéticos.
