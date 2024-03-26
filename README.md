# Projeto DSMovie

O projeto DSMovie é um sistema Fullstack desenvolvido durante a Semana Spring React - 9 a 15 de Maio de 2022, promovida pela Escola de programação DevSuperior.
As principais tecnologias utilizadas foram Java com ecossistema Spring Boot e TypeScript com a biblioteca React. O principal objetivo deste projeto é apresentar
ao usuário um catálogo de filmes onde cada usuário faz uma avaliação do filme escolhido entre 1 a 5 estrelas. Basicamente, ao escolher um filme, é aberta uma página 
com o filme escolhido, e o usuário insere seu e-mail e avaliação do filme. O banco de dados registra essa avaliação e a exibe para o usuário o número total de avaliações daquele e de outros filmes.

Segue o design Figma do projeto: 
https://www.figma.com/file/hpQuzpGHq2MmrI87xnfMoT/DSMovie1

## Modelo de domínio

Para termos uma visão da estrutura lógica do sistema, é apresentada um diagrama de classes contendo as relações entre as entidades do projeto.

![DomainModelDSMovie](https://github.com/rodrock95/dsmovie/assets/79290866/4b4f3728-b965-4ca3-9988-610687cc78c2)

## Lógica de Salvar uma avaliação

1. Informar email, id do filme e valor da avaliação (1 a 5).
2. Recuperar usuário do banco de dados pelo email. Se o usuário não existir, insira no banco.
3. Salvar a avaliação do usuário para o dado filme.
4. Recalcular a avaliação média do filme e salvar no banco de dados.

![logica](https://github.com/rodrock95/dsmovie/assets/79290866/ae0df225-9937-42d8-8853-ef82ada611a6)



