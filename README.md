# Test Técnico · Data Engineering + Microsoft Fabric

Test técnico de evaluación para perfiles de Data Engineering. Incluye:

- **Parte 1** — 35 preguntas tipo test (SQL, Arquitecturas, Orquestación, Cloud, Calidad, Fabric)
- **Parte 2** — 8 preguntas de respuesta libre
- **Parte 3** — 6 ejercicios SQL prácticos (lectura, corrección, escritura)
- **Parte 4** — 4 snippets de Python para analizar

## Despliegue en GitHub Pages

### 1. Sube el repositorio a GitHub

```bash
git init
git add .
git commit -m "Initial test"
git branch -M main
git remote add origin https://github.com/TU_USUARIO/de-test.git
git push -u origin main
```

### 2. Activa GitHub Pages

Ve a **Settings → Pages → Source: Deploy from branch → main / root**.

La URL del test será: `https://TU_USUARIO.github.io/de-test/`

### 3. Configura Formspree (para recibir las respuestas)

1. Crea cuenta gratuita en [formspree.io](https://formspree.io)
2. Crea un nuevo Form
3. Copia el endpoint (formato: `https://formspree.io/f/XXXXXXXX`)
4. En `index.html`, busca la línea:
   ```
   const FORMSPREE_ENDPOINT = 'https://formspree.io/f/YOUR_FORM_ID';
   ```
   Y reemplaza `YOUR_FORM_ID` con tu ID real.

El plan gratuito de Formspree permite **50 envíos/mes**, más que suficiente.

### 4. Envía el enlace a los candidatos

Puedes usar la URL base o añadir el nombre por parámetro (cosmético):
```
https://TU_USUARIO.github.io/de-test/
```

## Qué recibe el entrevistador

Al finalizar, Formspree envía un email con:

- Nombre, email y experiencia del candidato
- **Puntuación automática del tipo test** (X/35)
- Respuestas completas de cada sección en texto plano
- Tiempo total de la prueba
- Número de cambios de pestaña detectados

## Medidas anti-trampa incluidas

- Click derecho deshabilitado
- Atajos de teclado (Ctrl+C, Ctrl+A, Ctrl+P, F12) bloqueados
- Detección de cambios de pestaña con contador
- Texto no seleccionable (excepto en las áreas de respuesta)
- Orden de preguntas tipo test aleatorizado en cada sesión
- Temporizador por sección (orientativo, no bloquea el envío)

## Personalización

### Cambiar los tiempos por sección

En `index.html`, busca:
```js
timers: [25*60, 20*60, 20*60, 15*60],
```
Valores en segundos para cada sección (test, abiertas, SQL, Python).

### Añadir/quitar preguntas

Edita los arrays `MC_QUESTIONS`, `OPEN_QUESTIONS`, `SQL_EXERCISES` y `PYTHON_EXERCISES` en el bloque `QUESTION DATA` del script.
