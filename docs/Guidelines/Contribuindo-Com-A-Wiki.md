---
parent: Guidelines
nav_order: 20
---
# Contribuindo com a Wiki

Olá! Aqui você vai encontrar passo-a-passos de como contribuir com a Wiki da Equipe.

## Seção 0: O que é a Wiki?

A Wiki é um espaço de registro de informações sobre a Equipe e seus projetos. Ela é hosteada no GitHub por meio do [GitHub Pages](https://pages.github.com/) no repositório [Equipe-Botcem.github.io](https://github.com/Equipe-Botcem/Equipe-Botcem.github.io). Qualquer membro da equipe pode contribuir com a Wiki, basta criar Issues e Pull Requests nesse mesmo repositório citado (se você não sabe o que é isso, recomendamos dar uma olhada no nosso [Guia Inicial](./Getting-Started.md)).

Cada página é facilmente criada e editada em arquivos Markdown. Assim que uma alteração é feita na branch principal, o Workflow do GitHub Pages atualiza o site automaticamente. Porém, é possível visualizar as alterações localmente com o [Jekyll](https://jekyllrb.com/) (mais detalhes adiante).

## Seção 1: Criando uma página

Para criar uma página, basta criar um arquivo Markdown na pasta `docs` com o nome da página. Por exemplo, se você quiser criar uma página chamada `Minha Primeira Página`, basta criar um arquivo chamado `Minha-Primeira-Pagina.md` na pasta `docs` (o nome do arquivo deve ser escrito preferencialmente em [Train-Case](https://en.wikipedia.org/wiki/Naming_convention_(programming)#Examples_of_multiple-word_identifier_formats)).

O link final para essa página, após finalizada, será `https://equipe-botcem.github.io/Minha-Primeira-Pagina/`. Pode-se criar subpastas para organizar melhor as páginas, por exemplo, `docs/Projeto-X/Minha-Primeira-Pagina.md`. Nesse caso, o link final será `https://equipe-botcem.github.io/Projeto-X/Minha-Primeira-Pagina/`. 

No início de cada arquivo Markdown, deve-se colocar o seguinte código yaml:

```yaml
---
has_children: false # Se essa página tiver subpáginas, colocar true
parent: NOME_DA_PAGINA_PAI # Caso essa página seja uma subpágina 
nav_order: NÚMERO_DA_ORDEM # O número da ordem é usado para ordenar as páginas na barra lateral
---
```

> Para mais detalhes, leia a [documentação do Just the Docs](https://just-the-docs.github.io/just-the-docs/docs/navigation-structure/) ou veja os arquivos Markdown já existentes na pasta [`docs`](https://github.com/Equipe-Botcem/Equipe-Botcem.github.io/tree/main/docs).

## Seção 2: Visualizando as alterações localmente

O próprio GitHub fornece um tutorial de como testar as alterações localmente [aqui](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/testing-your-github-pages-site-locally-with-jekyll). 

Mas em resumo, é necessário instalar o Jekyll. Para isso, siga as [instruções de instalação](https://jekyllrb.com/docs/installation/) no site oficial de acordo com seu Sistema Operacional.

Após a instalação, basta executar o comando `bundle install` na pasta `docs` do repositório seguido com `bundle exec jekyll serve`. O site será hosteado localmente na porta 4000. Para acessar, basta abrir o navegador e digitar [`localhost:4000`](http://localhost:4000).

> Qualquer alteração nos arquivos `Gemfile` ou `Gemfile.lock` deve ser commitada com as alterações na Wiki.
