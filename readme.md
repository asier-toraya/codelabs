# Mis Codelabs

Este repositorio contiene una colección de **Codelabs** creados con la herramienta [Google Codelab Tools (claat)](https://github.com/googlecodelabs/tools).

Cada carpeta dentro de este repositorio corresponde a un codelab exportado, con su propio `index.html`, pasos, recursos y estructura necesaria para ser visualizado en la web.

---

## Objetivo del repositorio

El propósito de este repositorio es **alojar y publicar tutoriales interactivos** (codelabs) a través de **GitHub Pages**, de forma que cualquiera pueda acceder a ellos desde un navegador sin necesidad de servidores adicionales.

Ejemplo de publicación: `https://<tu-usuario>.github.io/mis-codelabs/`

```
mis-codelabs/
├── index.html ← Página principal con enlaces a los codelabs
├── mi-primer-codelab/ ← Codelab 1 (generado por claat)
│ ├── index.html
│ ├── step-1.html
│ ├── step-2.html
│ └── img/
└── otro-codelab/ ← Codelab 2 (otro ejemplo)
├── index.html
└── ...
```
Cada subcarpeta (`mi-primer-codelab/`, `otro-codelab/`, etc.) es el resultado del comando `claat export`.

---

## Cómo generar un nuevo codelab

1. Crea un archivo Markdown, por ejemplo `mi-nuevo-codelab.md`, con los metadatos requeridos:

   ```markdown
   summary: Mi nuevo codelab
   id: mi-nuevo-codelab
   categories: ejemplo, tutorial
   environments: Web
   status: Published
   authors: Tu Nombre

   # Mi nuevo Codelab

   ## Introducción
   Este es un codelab de ejemplo.
   ```
2. Usa la herramienta claat para exportarlo:
    ```
    claat export mi-nuevo-codelab.md
    ```
    Esto generará una carpeta mi-nuevo-codelab/ con todos los archivos listos para la web.
3. Mueve esa carpeta dentro de este repositorio (mis-codelabs/) y añade un enlace en index.html.