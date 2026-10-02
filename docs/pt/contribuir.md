# Contribuir

O site é construído com [MkDocs Material](https://squidfunk.github.io/mkdocs-material/) a partir de arquivos Markdown no GitHub. Qualquer membro da Rede pode propor alterações.

## :material-lightbulb-on-outline: Formas de participar

<div class="grid cards" markdown>

-   :material-teach:{ .lg .middle } __Ministrar um curso__

    ---

    Proponha um tema, prepare o material com o [modelo](cursos/plantilla/index.md) e nós publicamos aqui.

-   :material-domain:{ .lg .middle } __Sediar__

    ---

    Sua instituição pode receber uma edição presencial de um curso.

-   :material-translate:{ .lg .middle } __Traduzir__

    ---

    Ajude a manter as páginas em espanhol e português.

-   :material-bug-outline:{ .lg .middle } __Corrigir erros__

    ---

    Algum comando não funciona ou um link está quebrado? Abra uma *issue*.

</div>

## :material-folder-outline: Organização do repositório

```text
biogenomas-cursos/
├── mkdocs.yml              # configuração e menu do site
├── docs/
│   ├── es/                 # páginas em espanhol (idioma principal)
│   │   ├── cursos/
│   │   │   └── nome-do-curso/index.md
│   │   ├── calendario.md
│   │   └── ...
│   ├── pt/                 # as mesmas páginas, em português
│   ├── assets/             # logo e fotos da equipe (compartilhados)
│   └── stylesheets/extra.css
└── data/                   # dados de exemplo pequenos
```

!!! important "Regra de ouro do bilinguismo"
    Cada página existe com **o mesmo nome de arquivo** em `docs/es/` e `docs/pt/`. Se uma página ainda não tiver tradução, o site mostra a versão em espanhol.

## :material-source-branch: Fluxo de trabalho

1. Crie um branch ou um *fork* do repositório.
2. Edite ou adicione os arquivos `.md`.
3. Visualize localmente:

    ```bash
    pip install -r requirements.txt
    mkdocs serve        # abra http://127.0.0.1:8000
    ```

4. Abra um *pull request*. Quando aceito na `main`, o GitHub Actions publica o site automaticamente.

## :material-check-all: Boas práticas para os cursos

- Arquivos > 50 MB vão para o **Zenodo**, não para o repositório.
- Informe as **versões** dos softwares usados.
- Prefira dados de exemplo pequenos, que rodem em um notebook.
- Inclua a **licença** e como citar o material.
