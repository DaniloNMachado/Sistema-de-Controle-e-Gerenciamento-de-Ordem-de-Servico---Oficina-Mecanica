# Sistema de Controle e Gerenciamento de Ordem de Serviço - Oficina Mecânica

## Descrição do Projeto
Este projeto consiste na criação de um esquema conceitual para gerenciar ordens de serviço (OS) em uma oficina mecânica. Ele foi desenvolvido para atender às principais necessidades de registro, controle e execução de serviços realizados em veículos, proporcionando um fluxo organizado e eficiente.

## Objetivo
Implementar um sistema de banco de dados que permita:
- Gerenciar clientes, veículos, ordens de serviço, equipes de mecânicos, peças e serviços;
- Registrar autorizações dos clientes para execução dos serviços;
- Rastrear o histórico de status das ordens de serviço ao longo do processo;
- Calcular corretamente os valores de serviços e peças associados a cada OS.

# Estrutura Conceitual
## Clientes
- Cada cliente pode ter vários veículos registrados;
- Dados: Nome, Endereço, Documento (CPF/CNPJ).

## Veículos
- Relacionados aos clientes, com informações como modelo, marca, cor e tipo de serviço;
- Cada veículo está associado às ordens de serviço geradas na oficina.

## Equipe de Mecânicos
- Agrupamento de mecânicos com especialidades específicas para avaliação e execução dos serviços;
- Dados: Nome da equipe, nome, endereço e especialidade dos mecânicos.

## Ordem de Serviço (OS)
- Inclui informações como número, data de emissão, data de conclusão, valor total, status e autorização do cliente;
- Relaciona múltiplos serviços e peças executados pela equipe.

## Serviços
- Baseados em uma tabela de referência de mão-de-obra, calculados de acordo com o tipo de serviço prestado.

## Peças
- Cada OS pode incluir várias peças, com valores e quantidades calculados para compor o custo total.

## histórico de Status
- Registra alterações no status das ordens de serviço, como "Pendente", "Em andamento", "Concluído" e "Cancelado".

# Principais Funcionalidades
1. Registro de Autorizações:
  - Garantir que cada serviço seja executado apenas após autorização do cliente.
2. Rastreamento de histórico:
  - Monitorar alterações no status das ordens de serviço.
3. Gerenciamento de peças:
  - Permitir o cálculo exato do custo total considerando quantidade e valor unitário.
4. Relacionamento Dinâmico:
  - Conectar clientes, veículos, mecânicos, serviços e peças de forma integrada.

## Ferramentas Utilizadas
MySQL Workbench: Utilizado para modelagem e implementação do banco de dados.

# Imagem do projeto
![Projeto conceitual de Banco de Dados - Macanico - GIT](https://github.com/user-attachments/assets/779191a7-506f-411b-a823-f08134f2c1a1)


