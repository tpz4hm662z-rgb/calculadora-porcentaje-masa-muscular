# 🧰 sistema Herramientas360 v3.0

> Base visual oficial para el desarrollo de todas las herramientas de Herramientas360.

---

# 📖 Descripción

sistema Herramientas360 es la base oficial utilizada para crear todas las herramientas del proyecto Herramientas360.

Su objetivo es permitir desarrollar nuevas herramientas de forma rápida, manteniendo siempre la misma calidad, estructura, diseño y optimización SEO.

Todas las herramientas creadas a partir de esta base visual comparten:

- Diseño responsive
- SEO optimizado
- Accesibilidad
- Arquitectura modular
- Código reutilizable
- Buenas prácticas
- Estructura profesional

---

# 🎯 Objetivos de la base visual

La base visual ha sido diseñada para que crear una nueva herramienta sea un proceso sencillo.

El flujo de trabajo ideal es:

1. Duplicar la base visual.
2. Cambiar la configuración.
3. Escribir el cálculo.
4. Publicar.

Sin necesidad de volver a diseñar la estructura HTML, CSS o JavaScript.

---

# 🚀 Filosofía del proyecto

Herramientas360 sigue una filosofía muy sencilla:

> Crear herramientas útiles, rápidas y gratuitas.

Cada herramienta debe cumplir estos principios:

- Fácil de utilizar.
- Compatible con cualquier dispositivo.
- Carga rápida.
- Diseño limpio.
- Información útil.
- Código fácil de mantener.

---

# 📂 Estructura del proyecto

```text
herramientas360-v3/

css/
    style.css

js/
    config.js
    core.js
    script.js

img/
icons/

README.md
ARQUITECTURA.md
GUIA-DESARROLLO.md
H360-DESIGN-SYSTEM.md

robots.txt
sitemap.xml
.gitignore

index.html
```

---

# 📁 Descripción de cada archivo

## index.html

Contiene toda la estructura HTML de la herramienta.

Debe mantenerse limpio.

No debe contener lógica JavaScript.

---

## style.css

Toda la apariencia visual.

No debe contener estilos específicos de una herramienta concreta siempre que puedan reutilizarse.

---

## config.js

Centro de configuración.

Aquí se modifican:

- nombre
- icono
- categoría
- unidades
- mensajes
- resultados
- comportamiento
- formato
- configuración general

No debe contener funciones.

---

## core.js

Motor reutilizable.

Incluye todas las funciones comunes:

- validaciones
- formularios
- resultados
- errores
- scroll
- formatos
- utilidades
- accesibilidad

Nunca debe contener cálculos específicos.

---

## script.js

Únicamente contiene la lógica de la herramienta.

Debe ser el archivo más pequeño de todos.

Idealmente solo cambiará la función:

```javascript
function calcular(datos){

}
```

---

## robots.txt

Configuración para motores de búsqueda.

---

## sitemap.xml

Mapa del sitio.

Cada herramienta tendrá su propio sitemap.

---

# 🧱 Arquitectura

La arquitectura oficial es:

config.js

↓

core.js

↓

script.js

↓

index.html

Cada archivo tiene una única responsabilidad.

Nunca se deben mezclar responsabilidades entre ellos.
---

# 🚀 Crear una nueva herramienta

Todas las herramientas de Herramientas360 deben seguir siempre el mismo proceso.

## Paso 1

Duplicar la carpeta de la base visual.

Renombrar la carpeta con el nombre del nuevo proyecto.

Ejemplo:

calculadora-imc

calculadora-tmb

calculadora-calorias

---

## Paso 2

Actualizar los datos del proyecto.

Modificar:

- Nombre de la herramienta.
- Categoría.
- Icono.
- Descripción SEO.
- URL.
- Fecha de actualización.

La mayoría de estos cambios se realizan desde:

config.js

e index.html

---

## Paso 3

Modificar el formulario.

Editar únicamente los campos necesarios.

Añadir o eliminar inputs según la herramienta.

No modificar la estructura general.

---

## Paso 4

Programar el cálculo.

Toda la lógica debe implementarse únicamente dentro de:

script.js

En concreto dentro de:

```javascript
function calcular(datos){

}
```

No modificar core.js.

---

## Paso 5

Comprobar resultados.

Verificar:

- cálculo correcto
- formato
- unidades
- mensajes
- interpretación
- recomendaciones

---

## Paso 6

Actualizar SEO.

Revisar:

- title

- description

- canonical

- Open Graph

- Twitter Cards

- datos estructurados

---

## Paso 7

Actualizar robots.txt

Cambiar:

calculadora-porcentaje-masa-muscular

---

## Paso 8

Actualizar sitemap.xml

Modificar:

URL

Fecha

---

## Paso 9

Añadir imagen preview

Guardar:

img/preview.jpg

Será utilizada por:

Open Graph

Twitter

Compartir enlaces

---

## Paso 10

Probar la herramienta completamente.

Nunca publicar sin realizar pruebas.

---

# ✅ Checklist antes de publicar

Comprobar:

□ HTML válido

□ CSS correcto

□ JavaScript sin errores

□ Responsive

□ SEO actualizado

□ Robots actualizado

□ Sitemap actualizado

□ Iconos

□ Preview

□ Analytics

□ Accesibilidad

□ Enlaces internos

□ Footer

□ Resultado correcto

□ Reinicio correcto

□ Formularios funcionando

---

# 🌐 Publicación

Una vez finalizada:

1.

Commit

↓

2.

Push

↓

3.

GitHub Pages

↓

4.

Comprobar publicación

↓

5.

Enviar sitemap a Search Console

↓

6.

Solicitar indexación

---

# 📊 Google Analytics

Antes de publicar verificar:

- ID correcta

- Eventos funcionando

- Usuario en tiempo real

- Sin errores en consola

---

# 🔍 Google Search Console

Después de publicar:

Enviar:

sitemap.xml

Solicitar indexación de:

Página principal

---

# 🧪 Pruebas obligatorias

Comprobar:

Móvil

Tablet

Ordenador

Chrome

Safari

Edge

Firefox

También revisar:

Modo claro

Modo oscuro (si existe)

Orientación vertical

Orientación horizontal

---

# 🛠 Buenas prácticas

Nunca duplicar código.

Nunca modificar core.js para una única herramienta.

Toda configuración debe ir en config.js.

Toda lógica debe ir en script.js.

Toda estructura debe permanecer en index.html.

Todo estilo debe permanecer en style.css.

Mantener siempre la misma arquitectura.
---

# 📝 Convenciones de código

Para mantener una base de código uniforme, todas las herramientas deben seguir estas normas.

## HTML

- Utilizar HTML5 semántico.
- Mantener comentarios por secciones.
- Respetar la estructura oficial de la base visual.
- No añadir estilos inline.

---

## CSS

- Utilizar variables CSS.
- Mantener la nomenclatura existente.
- Evitar duplicar estilos.
- Mantener diseño responsive.

---

## JavaScript

Separación estricta de responsabilidades.

config.js

↓

Configuración

core.js

↓

Motor reutilizable

script.js

↓

Lógica de la herramienta

Nunca mezclar responsabilidades.

---

# 📌 Convenciones de nombres

Repositorios:

calculadora-imc

calculadora-tmb

calculadora-iva

Nunca utilizar espacios.

Siempre minúsculas.

Separar palabras con guiones.

---

# 🔖 Versionado

La base visual utiliza versionado semántico.

Ejemplos:

v3.0 Stable

v3.1

v3.2

v4.0

Cambios pequeños:

Incrementar versión menor.

Cambios de arquitectura:

Incrementar versión principal.

---

# 📅 Mantenimiento

Antes de crear una nueva herramienta comprobar:

- Última versión de la base visual.
- Posibles mejoras pendientes.
- Compatibilidad con herramientas anteriores.

No modificar la arquitectura sin una necesidad real.

---

# 🚀 Roadmap

Posibles mejoras futuras:

- Exportar PDF.

- Compartir resultados.

- Copiar al portapapeles.

- LocalStorage avanzado.

- Historial de cálculos.

- Internacionalización (i18n).

- Tema oscuro.

- PWA.

- Modo sin conexión.

Estas mejoras deberán incorporarse únicamente en nuevas versiones de la base visual.

---

# 📋 Filosofía de Herramientas360

La prioridad del proyecto no es crear una base visual perfecta.

La prioridad es crear herramientas útiles.

La base visual existe para acelerar el desarrollo.

Una vez publicada una versión estable:

No modificar la arquitectura salvo necesidad real.

Las mejoras futuras deberán planificarse para nuevas versiones.

---

# 🤝 Flujo oficial de trabajo

Nueva idea

↓

Duplicar base visual

↓

Configurar proyecto

↓

Desarrollar cálculo

↓

Realizar pruebas

↓

Publicar

↓

Actualizar portal

↓

Enviar sitemap

↓

Solicitar indexación

↓

Analizar resultados

---

# 🎯 Objetivo del proyecto

Crear una colección de herramientas gratuitas, rápidas y útiles que ayuden a miles de personas en su día a día.

Cada nueva herramienta debe aportar valor real.

La calidad siempre estará por encima de la cantidad.

---

# 🏁 Estado de la base visual

**sistema Herramientas360 v3.0**

Estado:

✅ Finalizada

Arquitectura estable.

Preparada para el desarrollo de nuevas herramientas.

---

# © Autor

Proyecto desarrollado por

**José Carlos Núñez Florido**

con la asistencia de ChatGPT.

© 2026 Herramientas360

Todos los derechos reservados.

## URL pública

[Abrir la Calculadora de Porcentaje de Masa Muscular Pro](https://tpz4hm662z-rgb.github.io/calculadora-porcentaje-masa-muscular/)

Repositorio: [tpz4hm662z-rgb/calculadora-porcentaje-masa-muscular](https://github.com/tpz4hm662z-rgb/calculadora-porcentaje-masa-muscular)


## Versión publicada

1.0.1 — 31 de julio de 2026.
