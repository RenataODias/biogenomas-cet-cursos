# Contribuir

El sitio se construye con [MkDocs Material](https://squidfunk.github.io/mkdocs-material/) a partir de archivos Markdown en GitHub. Cualquier miembro de la Red puede proponer cambios.

## :material-lightbulb-on-outline: Formas de participar

<div class="grid cards" markdown>

-   :material-teach:{ .lg .middle } __Impartir un curso__

    ---

    Propón un tema, prepara el material con la [plantilla](cursos/plantilla/index.md) y lo publicamos aquí.

-   :material-domain:{ .lg .middle } __Ser sede__

    ---

    Tu institución puede recibir una edición presencial de un curso.

-   :material-translate:{ .lg .middle } __Traducir__

    ---

    Ayuda a mantener las páginas en español y portugués.

-   :material-bug-outline:{ .lg .middle } __Corregir errores__

    ---

    ¿Un comando no funciona o un enlace está roto? Abre una *issue*.

</div>

## :material-folder-outline: Organización del repositorio

```text
biogenomas-cursos/
├── mkdocs.yml              # configuración y menú del sitio
├── docs/
│   ├── es/                 # páginas en español (idioma principal)
│   │   ├── cursos/
│   │   │   └── nombre-del-curso/index.md
│   │   ├── calendario.md
│   │   └── ...
│   ├── pt/                 # mismas páginas, en portugués
│   ├── assets/             # logo y fotos del equipo (compartidos)
│   └── stylesheets/extra.css
└── data/                   # datos de ejemplo pequeños
```

!!! important "Regla de oro del bilingüismo"
    Cada página existe con **el mismo nombre de archivo** en `docs/es/` y `docs/pt/`. Si una página aún no tiene traducción, el sitio muestra la versión en español.

## :material-source-branch: Flujo de trabajo

1. Crea una rama o un *fork* del repositorio.
2. Edita o agrega los archivos `.md`.
3. Visualiza localmente:

    ```bash
    pip install -r requirements.txt
    mkdocs serve        # abre http://127.0.0.1:8000
    ```

4. Abre un *pull request*. Al aceptarse en `main`, GitHub Actions publica el sitio automáticamente.

## :material-check-all: Buenas prácticas para los cursos

- Archivos > 50 MB van a **Zenodo**, no al repositorio.
- Indica las **versiones** del software usado.
- Prefiere datos de ejemplo pequeños que se ejecuten en un portátil.
- Incluye la **licencia** y cómo citar el material.
