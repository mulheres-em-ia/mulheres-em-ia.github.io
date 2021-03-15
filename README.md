
# Como fazer postagens no site do MIA via github pages

O site do MIA é uma [página do Github](https://docs.github.com/pt/github/working-with-github-pages/creating-a-github-pages-site).
O github pages é uma funcionalidade do Github que te permite criar uma página usando Markdown. Não sabe o que é Markdown? Dá uma olhada [aqui](https://guides.github.com/features/mastering-markdown/) :wink:

## Quero criar uma nova página

É muito importante que você siga o tutorial a risca, pois o Jenkyll que roda por trás do Github Pages que faz toda a mágica. 

Em _posts crie um novo arquivo com a data da publicação (é importante que a data esteja no presente ou passado, caso contrário o post não aparecerá). Ex de nome: 2020-12-07-primeiro-evento-mia.markdown


Dentro deste arquivo é importante que você comece tudo sempre com esse código:

```
---
layout: post
title: "Titulo que você quer entre aspas"
author: Seu nome
subtitle: "Qualquer subtitulo que você queira entre aspas"
date: 2021-03-15 14:24:00 -0300
---
```
O formato da data deve respeitar o padrão YYYY-MM-DD HH-mm-ss -0300

Depois disso é só escrever tudo em markdown que o Jenkyl fará a magia para você. Se tiver dúvidas pode consultar [essa página](https://github.com/mulheres-em-ia/mulheres-em-ia.github.io/blob/main/_posts/2020-12-07-primeiro-evento-mia.markdown).

## Quero editar uma página existente

Sempre que for editar uma página é muito importante que você vá à pasta _posts e não na pasta que contém o html. Mexer diretamente no html não terá efeito pois ao fazer o merge na master você faz "deploy" de uma nova versão do site e ele sobrescreverá a sua página html com o markdown que ele possui.
