# API de Cadastro de Médicos para Clinica Médica

Esta é uma API simples de estudo que permite o cadastro, listagem, atualização e exclusão de médicos em uma clínica médica. Os médicos são cadastrados com informações essenciais, incluindo nome, e-mail, telefone, CRM, especialidade e endereço completo. Além disso, a API implementa regras de negócio específicas para garantir a integridade dos dados.

## Configuração do Projeto

Certifique-se de ter as seguintes dependências configuradas em seu ambiente de desenvolvimento:
* Java 17
* Maven
* Banco de Dados MySQL
* Ambiente de Desenvolvimento Spring Boot

## Dependências do Projeto

As dependências do projeto estão definidas no arquivo pom.xml.

* Spring Boot Starter Web
* Spring Boot DevTools
* Lombok
* Spring Boot Starter Test
* Spring Boot Starter Data JPA
* Spring Boot Starter Validation
* Flyway para migração de banco de dados
* MySQL Connector

Certifique-se de que todas essas dependências estejam configuradas corretamente antes de iniciar o projeto.

## Configuração do Banco de Dados

A configuração do banco de dados MySQL é feita no arquivo application.properties. Você deve configurar as propriedades do banco de dados, como URL, nome de usuário e senha, de acordo com o seu ambiente.

spring.datasource.url=jdbc:mysql://localhost:3306/nome_do_banco
spring.datasource.username=seu_usuario
spring.datasource.password=sua_senha

## Funcionalidades da API

* Cadastro de Médicos (POST)

Todas as informações são obrigatórias, exceto "número" e "complemento" do endereço.
O e-mail, CRM e especialidade não podem ser alterados posteriormente.

* Listagem de Médicos (GET)

A lista é ordenada pelo nome do médico em ordem crescente.

* Atualização de Médicos (PUT)

Apenas o nome, telefone e endereço podem ser atualizados.
E-mail, CRM e especialidade não podem ser alterados.

* Exclusão de Médicos (DELETE)

A exclusão não apaga os dados do médico, apenas marca-o como "inativo" no sistema.

## Executando a Aplicação

A aplicação será iniciada na porta padrão 8080. Certifique-se de ajustar as configurações de porta no arquivo application.properties conforme necessário.

## Conclusão
Este README fornece uma visão geral completa do projeto da API de cadastro de médicos. Certifique-se de configurar corretamente o ambiente, o banco de dados e as dependências antes de executar a aplicação. Aproveite o desenvolvimento e a utilização da sua API para gerenciar médicos em uma clínica médica de forma eficiente.

## Contatos

• E-mail: crisoenning@gmail.com

• Instagram: instagram.com/cristopher_oenning

• Github: github.com/cris-oenning
