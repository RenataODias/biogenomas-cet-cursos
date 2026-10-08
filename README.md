# BioGenomas · Cursos

Sitio de cursos del **Comité de Formación y Transferencia de Conocimiento – Red de Genomas Neotropicales (Red BioGenomas)**.
Site de cursos do **Comitê de Formação e Transferência de Conhecimento – Rede de Genomas Neotropicais (Rede BioGenomas)**.

🌐 https://RenataODias.github.io/biogenomas-cet-cursos/

## Estrutura

```
mkdocs.yml               configuração, menu e traduções do menu
docs/es/                 páginas em espanhol (idioma padrão)
docs/pt/                 mesmas páginas em português (mesmos nomes de arquivo)
docs/assets/             logo e fotos da equipe
docs/stylesheets/        CSS (cores do site)
data/                    dados de exemplo pequenos
.github/workflows/       publicação automática no GitHub Pages
```

## Rodar localmente

```bash
pip install -r requirements.txt
mkdocs serve
```

## Publicação

Cada `push` na branch `main` dispara o GitHub Actions, que gera o site na branch `gh-pages`.
Na primeira vez: **Settings → Pages → Source: Deploy from a branch → `gh-pages` / root**.

## Licença

Conteúdo: [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) · Código: [MIT](https://opensource.org/licenses/MIT)
