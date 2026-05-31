# Test Técnico · Data Engineering + Microsoft Fabric

Este repositorio contiene una prueba técnica web para evaluar candidatos de Data Engineering en un único flujo, combinando conocimientos teóricos y capacidad práctica.

## En qué consiste la prueba

La evaluación está dividida en 4 bloques:

- **Parte 1**: 28 preguntas tipo test sobre SQL, arquitectura de datos, orquestación, cloud, calidad y Microsoft Fabric.
- **Parte 2**: 4 preguntas abiertas para valorar criterio técnico, capacidad de síntesis y comunicación.
- **Parte 3**: 6 ejercicios SQL prácticos (lectura, corrección y escritura de consultas).
- **Parte 4**: 4 fragmentos de Python para analizar y razonar.

## Objetivo de evaluación

La prueba busca medir de forma equilibrada:

- Base conceptual de ingeniería de datos.
- Soltura resolviendo problemas reales de SQL.
- Capacidad de análisis de código en Python.
- Claridad al argumentar decisiones técnicas.

## Funcionamiento general

- Es una prueba de una sola sesión, pensada para completarse de principio a fin.
- Incluye temporizadores orientativos por bloque para guiar el ritmo.
- El test tipo test se puntúa automáticamente.
- Las respuestas abiertas, SQL y Python quedan registradas para revisión cualitativa.

## Información que obtiene el entrevistador

Al finalizar una candidatura, se recopila:

- Datos básicos del candidato (identificación y experiencia declarada).
- Resultado automático del bloque tipo test.
- Respuestas completas en formato texto del resto de secciones.
- Tiempo total consumido en la prueba.
- Número de cambios de pestaña detectados durante la sesión.

## Mecanismos de integridad de la prueba

El formulario incorpora medidas de control para reducir ayudas externas durante la realización:

- Bloqueo de acciones de inspección y copia más comunes.
- Detección de cambios de pestaña con contador.
- Orden aleatorio de preguntas tipo test por sesión.
- Restricción de selección de texto fuera de áreas de respuesta.

## Estructura del repositorio

- `index.html`: aplicación completa de la prueba (estructura, estilo, lógica y banco de preguntas).
- `README.md`: descripción funcional del proyecto.
