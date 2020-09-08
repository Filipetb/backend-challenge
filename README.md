# Desafio | Backend Developer | Wecont

Olá! Seja bem vindo ao teste para a vaga de Backend Developer.

Preparamos um teste que abordará seus conhecimentos em PHP e REST API. Você será encaixado na vaga de acordo com seu resultado.

A necessidade é desenvolver o projeto "Gerencia Faturas", onde o usuráio pode gerenciar suas próprias faturas geradas.

## Instruções para entrega

* Versione, com git, e hospede seu código em algum serviço de sua preferência: github, bitbucket, gitlab ou outro.
* Crie um README com instruções claras sobre como executar sua obra.
* Envie um email com o link do seu repositório para guilherme.brant@wecont.net
* Dúvidas podem ser enviadas para o mesmo email acima.

## API

Você terá que implementar uma REST API para gerenciar as faturas de usuários.

É importante ter autenticação do usuário e paginação das faturas.

Qualquer tipo de dado deve sempre ser retornado no formato JSON.

## Entities

A API deverá ter usuários e faturas. Um usuário poderá ter uma ou mais faturas, enquanto uma fatura deverá percentecer somente à um usuário.

**Usuários possuem:**

* Email (Email para autenticação)
* Senha (Senha para autenticação)

**Faturas possuem:**

* Status (Podem ter os seguintes valores: Paga | Aberta | Atrasada)
* Vencimento (Data de vencimento da fatura)
* URL (Link para visualização da fatura)

*Todos os campos são obrigatórios e não nulos*
*Não é necessário realizar upload de faturas, nem mesmo links reais para visualização das mesmas*

## Rotas

Deverá implementar rotas que contemplem os seguintes objetivos:

- Autenticar um usuário
- Mostrar as informações do usuário autenticado.
- CRUD de faturas do usuário autenticado (um usuário não deverá ter acesso à faturas de outro).
- A rota de ler faturas deverá ter paginação, sendo, por padrão, 5 faturas por página.
- Com excessão da rota de Autenticar um usuário, as demais deverão serem acessadas somente por usuários autenticados.

## Requisitos

* O projeto deverá ser entregue na linguagem PHP (7 ou superior).
* Deve-se utilizar Laravel (7 ou superior) ou Slim (3.12 ou suporior) como frameworks.
* Use mysql, mariadb ou SQLite para persistir os dados.
* Use HTTP Basic Auth e/ou JWT para autenticar os usuários.

## Requisitos Opcionais

* Padronização do código: seguir diretrizes de padrão de projetos.

## Critérios de avaliação

* Fidelidade às funcionalidades solicitadas;
* Clareza de nomenclatura do código;
* Organização do código;
* Requisitos Opcionais;

## Não conseguiu fazer tudo?

A sua forma de priorizar a entrega também vai ser considerada. Documente em um arquivo a parte o que você conseguiu e não conseguiu implementar, descrevendo porque você preferiu priorizar desta maneira.
