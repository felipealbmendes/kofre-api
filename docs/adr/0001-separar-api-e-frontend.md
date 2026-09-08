# ADR-0001: Separar API e frontend em repositórios distintos

## Status
Aceito

## Contexto
Para amparar uma possível estrutura multi-plataforma (web/app/desktop) e escalar
atualizações de interface do projeto, definimos que a API deverá poder ser consumida
por diferentes projetos.

## Decisão
Separar os repositórios de back-end e front-end.

## Alternativas consideradas
Ter um repositório único com back-end e front-end.

## Consequências
Com essa decisão, teremos um projeto de API independente que centraliza toda a regra
do projeto, e podemos, a partir disso, ter projetos de front-end mais fáceis de serem
atualizados e um suporte a diversas interfaces que podem consumir os endpoints da
aplicação principal. Em contrapartida, teremos o trabalho de manter atualizações em
mais de um projeto, assim como estruturas de versionamento e de pipelines de CI/CD
distintas.
