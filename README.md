# 🏪 Sistema Cantina

**Sistema de gerenciamento de estoque e vendas para cantina escolar.**

Projeto acadêmico desenvolvido em Python com o objetivo de facilitar o controle de produtos, movimentações de estoque, vendas e datas de validade em uma cantina escolar.

https://github.com/henriquethe
\

---

## 📑 Sumário

* [Sobre o projeto](#-sobre-o-projeto)
* [Objetivos](#-objetivos)
* [Funcionalidades](#-funcionalidades)
* [Usuários do sistema](#-usuários-do-sistema)
* [Tecnologias utilizadas](#-tecnologias-utilizadas)
* [Regras de negócio](#-regras-de-negócio)
* [Estrutura do sistema](#-estrutura-do-sistema)
* [Demonstração](#-demonstração)
* [Banco de dados e backup](#-banco-de-dados-e-backup)
* [Levantamento de requisitos](#-levantamento-de-requisitos)
* [Status do projeto](#-status-do-projeto)
* [Finalidade acadêmica](#-finalidade-acadêmica)
* [Participantes](#-participantes)

---

## 📋 Sobre o projeto

O **Sistema Cantina** é um projeto acadêmico voltado ao desenvolvimento de uma solução para gerenciamento de estoque e vendas em uma cantina escolar.

A proposta surgiu da necessidade de melhorar o controle dos produtos, reduzindo problemas comuns no gerenciamento manual, como falta de mercadorias, desperdício de alimentos e divergências entre o estoque físico e os registros.

O sistema busca centralizar as informações em uma interface organizada, permitindo acompanhar os produtos cadastrados, registrar movimentações e consultar informações importantes para o funcionamento da cantina.

## 🎯 Objetivos

O principal objetivo é desenvolver uma aplicação que facilite o gerenciamento das operações diárias da cantina escolar.

Entre os objetivos específicos estão:

* Organizar o cadastro dos produtos.
* Controlar as entradas e saídas do estoque.
* Registrar as vendas e atualizar as quantidades automaticamente.
* Identificar produtos com estoque abaixo do mínimo.
* Acompanhar lotes e datas de validade.
* Disponibilizar informações para consulta e geração de relatórios.
* Reduzir erros no controle manual do estoque.

## ✨ Funcionalidades

O projeto contempla as seguintes funcionalidades:

| Funcionalidade            | Descrição                                                          |
| ------------------------- | ------------------------------------------------------------------ |
| Cadastro de produtos      | Registrar informações dos produtos comercializados.                |
| Controle de estoque       | Acompanhar as quantidades disponíveis.                             |
| Entrada de produtos       | Adicionar ao estoque as quantidades recebidas.                     |
| Saída de produtos         | Registrar perdas, vencimentos, danos e outras retiradas.           |
| Controle de vendas        | Registrar vendas e descontar automaticamente os produtos vendidos. |
| Alerta de estoque baixo   | Identificar produtos abaixo da quantidade mínima definida.         |
| Controle de validade      | Acompanhar lotes e datas de vencimento.                            |
| Pesquisa de produtos      | Facilitar a localização de itens cadastrados.                      |
| Relatórios                | Consultar informações sobre estoque, movimentações e vendas.       |
| Gerenciamento de usuários | Diferenciar os usuários e suas permissões de acesso.               |
| Backup                    | Criar cópias de segurança do banco de dados.                       |

> **Observação:** a disponibilidade de cada funcionalidade depende da implementação atual do sistema. Consulte a seção [Status do projeto](#-status-do-projeto).

## 👥 Usuários do sistema

O sistema foi planejado para atender a dois perfis principais.

### Responsável pela cantina

Responsável pelas operações diárias, incluindo:

* Cadastro e consulta de produtos.
* Registro de entradas e saídas.
* Registro de vendas.
* Acompanhamento das quantidades disponíveis.

### Direção da escola

Responsável pelo acompanhamento das informações e pela supervisão, incluindo:

* Consulta do estoque.
* Visualização dos relatórios.
* Acompanhamento das vendas.
* Verificação de produtos com estoque baixo.
* Consulta de produtos próximos do vencimento.

As permissões de cada perfil deverão ser aplicadas de acordo com as funcionalidades implementadas.

## 🛠️ Tecnologias utilizadas

| Tecnologia                        | Finalidade                                                          |
| --------------------------------- | ------------------------------------------------------------------- |
| [Python](https://www.python.org/) | Desenvolvimento da aplicação e implementação das regras de negócio. |
| [SQLite](https://www.sqlite.org/) | Armazenamento e consulta dos dados.                                 |
| [Git](https://git-scm.com/)       | Controle de versão do código-fonte.                                 |
| [GitHub](https://github.com/)     | Hospedagem do repositório e acompanhamento do desenvolvimento.      |

## 📐 Regras de negócio

O funcionamento do sistema deverá respeitar as seguintes regras:

1. Todo produto deve possuir as informações necessárias para seu cadastro.
2. Toda entrada deve aumentar a quantidade disponível.
3. Toda saída deve diminuir a quantidade disponível.
4. Toda venda registrada deve gerar a respectiva baixa no estoque.
5. O sistema não deve permitir que a quantidade em estoque fique negativa.
6. Cada produto pode possuir uma quantidade mínima definida.
7. Produtos abaixo do estoque mínimo devem gerar um alerta.
8. Os produtos podem ser organizados por lotes.
9. Os lotes podem possuir datas de validade.
10. Produtos próximos do vencimento devem ser identificados.
11. As movimentações devem ser registradas para permitir consultas posteriores.

## 🗂️ Estrutura do sistema

O sistema foi organizado conceitualmente em módulos que representam as principais operações da cantina.

* **Produtos:** cadastro, pesquisa e consulta de produtos.
* **Estoque:** controle das quantidades e movimentações.
* **Vendas:** registro das vendas e atualização do estoque.
* **Alertas:** identificação de estoque baixo e produtos próximos do vencimento.
* **Relatórios:** apresentação das informações para consulta.
* **Usuários:** gerenciamento dos acessos.
* **Banco de dados:** persistência das informações.

Essa divisão representa a organização funcional prevista para o projeto. A estrutura final dos arquivos e módulos dependerá da implementação do código-fonte.

## 🖥️ Demonstração

A seguir, algumas telas da interface desenvolvida para o sistema.

### Criação de conta

### Tela inicial

### Cadastro de produtos

### Protótipo inicial

O protótipo em papel foi utilizado para planejar a disposição das informações e os principais elementos do painel.

[📄 Visualizar o protótipo do painel](https://github.com/antoniorodrigues20082006-lab/Trabalho-python-/blob/main/Prot%C3%B3tipo%20no%20papel.jpeg)

## 🗄️ Banco de dados e backup

O projeto utiliza o SQLite como tecnologia prevista para persistência dos dados.

O banco de dados poderá armazenar informações relacionadas a:

* Produtos e categorias.
* Quantidades em estoque.
* Entradas e saídas.
* Vendas realizadas.
* Lotes e datas de validade.
* Usuários do sistema.

Também está prevista a criação periódica de cópias de segurança para reduzir o risco de perda das informações armazenadas.

A rotina de backup e os mecanismos de recuperação deverão ser validados durante a etapa de testes.

## 📝 Levantamento de requisitos

O levantamento de requisitos foi documentado a partir de uma entrevista simulada com inteligência artificial, representando o cenário de uma cantina escolar.

**Informações do levantamento:**

* **Estabelecimento de referência:** Escola Novo Futuro (ENF).
* **Responsável pela cantina no cenário:** Sara Ribeiro de Souza.
* **Responsável pelo levantamento:** Antonio Rodrigues da Silva Neto.
* **Data:** 23/09/2026.

📄 [Consultar o formulário de levantamento de requisitos](https://github.com/antoniorodrigues20082006-lab/Trabalho-python-/blob/main/Formulario_Cantina_Estoque.pdf)

> **Nota metodológica:** a entrevista foi simulada com IA para fins acadêmicos. Portanto, as informações representam um cenário de estudo, e não devem ser interpretadas como uma entrevista real realizada com uma funcionária do estabelecimento.

## 🚧 Status do projeto

O projeto encontra-se em desenvolvimento, com as seguintes etapas registradas:

* [x] Levantamento de requisitos.
* [x] Identificação dos usuários.
* [x] Definição das funcionalidades principais.
* [x] Criação do protótipo inicial do painel.
* [x] Modelagem do banco de dados.
* [x] Desenvolvimento do sistema.
* [x] Implementação do controle de estoque.
* [x] Implementação das vendas.
* [x] Implementação dos alertas.
* [ ] Implementação do backup.
* [x] Realização dos testes.
* [x] Finalização da documentação.

> As etapas marcadas como concluídas devem corresponder ao que já foi efetivamente implementado e validado no código.

## 🎓 Finalidade acadêmica

Este projeto está sendo desenvolvido como atividade acadêmica do curso de **Ciência da Computação**.

Seu propósito é aplicar conhecimentos de programação, banco de dados, levantamento de requisitos, modelagem de sistemas e desenvolvimento de interfaces em um problema prático.

O desenvolvimento também busca proporcionar experiência na organização de um projeto de software, desde a identificação do problema até a implementação e os testes da solução.

## 👥 Participantes

Projeto acadêmico desenvolvido em colaboração por:

* **Antonio Rodrigues da Silva Neto** — [GitHub](https://github.com/antoniorodrigues20082006-lab)
* **Henrique** — [GitHub](https://github.com/henriquethe)
* **José Vitor** _ [GitHub](https://github.com/Vmotovlogouslq)
---

*Sistema Cantina — Projeto acadêmico de gerenciamento de estoque para cantina escolar.*
