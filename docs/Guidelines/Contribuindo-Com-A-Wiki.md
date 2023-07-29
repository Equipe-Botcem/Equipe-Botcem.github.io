---
parent: Guidelines
nav_order: 20
---
# Contribuindo com a Wiki
{: .no_toc }

Olá! Aqui você vai encontrar passo-a-passos de como contribuir com a Wiki da Equipe.

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Seção 0: O que é a Wiki?

A Wiki é um espaço de registro de informações sobre a Equipe e seus projetos. Ela é hosteada no GitHub por meio do [GitHub Pages](https://pages.github.com/) no repositório [Equipe-Botcem.github.io](https://github.com/Equipe-Botcem/Equipe-Botcem.github.io). Qualquer membro da equipe pode contribuir com a Wiki, basta criar **Issues** e **Pull Requests** nesse mesmo repositório citado (se você não sabe o que é isso, recomendamos dar uma olhada no nosso [Guia Inicial](./Getting-Started.md)).

Cada página é facilmente criada e editada em **arquivos Markdown**. Assim que uma alteração é feita na branch principal, o Workflow do GitHub Pages atualiza o site automaticamente. Porém, é possível [**visualizar as alterações localmente**](#seção-1-visualizando-as-alterações-localmente) com o [Jekyll](https://jekyllrb.com/) (mais detalhes adiante).

## Seção 1: Visualizando as alterações localmente

É interessante visualizar as alterações localmente antes de commitá-las para a branch principal. O próprio GitHub fornece um tutorial de como testar as alterações localmente [aqui](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/testing-your-github-pages-site-locally-with-jekyll).

Mas **em resumo**, é necessário instalar o **Ruby** e o **Jekyll**. Para isso, siga as [instruções de instalação](https://jekyllrb.com/docs/installation/) no site oficial de acordo com seu Sistema Operacional.

> Para usuários **Windows**, o caminho mais fácil é instalar por meio do [RubyInstaller (Ruby + DevKit)](https://rubyinstaller.org/downloads/).\
> Para usuários **Ubuntu**, o caminho mais fácil é instalar por meio do [Gerenciador de Pacotes do Ubuntu](https://jekyllrb.com/docs/installation/ubuntu/).

Após a instalação, basta executar o comando `bundle install` a partir da pasta `docs` do repositório (`cd docs`) seguido de `bundle exec jekyll serve`. O site será hosteado localmente na porta 4000. Para acessar, basta abrir o navegador e digitar [`localhost:4000`](http://localhost:4000).

{: .highlight }
> Qualquer alteração nos arquivos `Gemfile` ou `Gemfile.lock` deve ser commitada com as alterações na Wiki.

## Seção 2: Criando uma página

Para criar uma página, basta criar um arquivo Markdown na pasta `docs` com o nome da página. Por exemplo, se você quiser criar uma página chamada `Minha Página`, basta criar um arquivo chamado `Minha-Pagina.md` dentro da pasta `docs` **(o nome do arquivo deve ser escrito preferencialmente em [<nobr>Train-Case</nobr>](https://en.wikipedia.org/wiki/Naming_convention_(programming)#Examples_of_multiple-word_identifier_formats))**. O link final para essa página, após finalizada, será `https://equipe-botcem.github.io/Minha-Pagina/`.

Para criar uma sub-página, basta criar uma página dentro de alguma seção, por exemplo, `docs/Projeto-X/Minha-Pagina`. O link final para essa página, após finalizada, será `https://equipe-botcem.github.io/Projeto-X/Minha-Pagina/`.

{: .highlight }

No início de cada arquivo Markdown, deve-se colocar o seguinte código yaml:

```yaml
---
parent: NOME_DA_PAGINA_PAI # Caso essa página seja uma sub-página 
nav_order: NÚMERO_DA_ORDEM  # Ordem que vai aparecer no menu à esquerda
title: TÍTULO  # O que vai aparecer no menu à esquerda
has_children: true  # Se possui sub-páginas
# permalink: /NOME_DA_PAGINA/  # Caso queira um link personalizado
---
```

{: .highlight }
> Para mais detalhes, leia a [documentação do Just the Docs](https://just-the-docs.github.io/just-the-docs/docs/navigation-structure/) ou veja os arquivos Markdown já existentes na pasta [`docs`](https://github.com/Equipe-Botcem/Equipe-Botcem.github.io/tree/main/docs).

## Seção 3: Criando uma seção

Pode-se também criar (sub)seções para melhor organizar as páginas, basta criar uma pasta com o nome da seção e, dentro dela, adicionar um arquivo `index.md`. Ele será a página inicial da seção, ou seja, ao clicar no link da seção, o usuário será redirecionado para essa página.

Além disso, ela funciona como uma página normal, ou seja, deve-se colocar o seguinte código yaml no início do arquivo:

```yaml
---
nav_order: NÚMERO_DA_ORDEM  # Ordem que vai aparecer no menu à esquerda
title: TÍTULO  # O que vai aparecer no menu à esquerda
has_children: true  # Se possui sub-páginas
# permalink: /NOME_DA_PAGINA/  # Caso queira um link personalizado
---
```
