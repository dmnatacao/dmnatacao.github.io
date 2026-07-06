# DM Natação — Site da Equipe

Site estático de resultados e desempenho da equipe de natação DM, gerado a partir do histórico consolidado em planilha (`DM_Natacao_Historico.xlsx`).

## Conteúdo

- Visão geral da equipe (KPIs, medalhas, participações)
- Página por atleta com histórico individual, melhores tempos e recordes
- Ranking, resultados e recordes por prova/categoria
- Galeria de fotos
- Alternância de tema claro/escuro

## Stack

Arquivo único (`index.html`), sem build step — HTML + CSS + JavaScript puro, com [Chart.js](https://www.chartjs.org/) via CDN para os gráficos. Todas as imagens (logo, fotos) estão embutidas em base64 no próprio arquivo, então não há dependência de assets externos além de fontes (Google Fonts) e do Chart.js.

## Publicação (GitHub Pages)

Este repositório é publicado via GitHub Pages a partir da branch `main` (raiz `/`). URL do site: preenchido após ativação do Pages.

## Privacidade

Os atletas da equipe incluem menores de idade. Por padrão, o site público **não exibe idade nem ano de nascimento** de atletas menores de 18 anos — apenas nome e categoria. Esses dados completos permanecem apenas na planilha interna (`DM_Natacao_Historico.xlsx`), que não faz parte deste repositório.

## Atualização de dados

Os dados de atletas e resultados vêm da planilha histórica do projeto. Ao atualizar a planilha, os dados correspondentes (`window.__DATA__`) neste `index.html` precisam ser regenerados/atualizados manualmente.
