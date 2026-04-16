# 📄 Folha de Pagamento em Java

Este projeto é uma aplicação Java em console que simula um sistema simples de folha de pagamento. O sistema permite cadastrar diferentes tipos de funcionários e calcular automaticamente seus salários de acordo com suas regras específicas, utilizando Programação Orientada a Objetos.

O projeto faz uso de herança, polimorfismo e classes abstratas, sendo ideal para fins acadêmicos e aprendizado da linguagem Java.

## 🧩 Tipos de Funcionários

O sistema trabalha com três tipos de funcionários:

- Funcionário Padrão  
  Possui salário fixo no valor de R$ 2000,00.

- Funcionário Comissionado  
  Possui salário base de R$ 2000,00 acrescido de uma comissão calculada a partir do valor total das vendas e do percentual informado.

- Funcionário de Produção  
  Possui salário base de R$ 2000,00 acrescido de um valor calculado com base na quantidade de peças produzidas e no valor por peça.

## 🛠 Tecnologias Utilizadas

- Java  
- Scanner para entrada de dados  
- ArrayList para armazenamento dos funcionários  
- Programação Orientada a Objetos (POO)

## 🧱 Estrutura do Projeto

O projeto é composto pelas seguintes classes:

- Funcionario (classe abstrata)  
- FuncionarioPadrao  
- FuncionarioComissionado  
- FuncionarioProducao  
- FolhaDePagamento (classe principal com menu interativo)

## 📋 Funcionalidades

- Cadastro de funcionários
- Cálculo automático do salário
- Listagem completa da folha de pagamento
- Exibição da quantidade total de funcionários cadastrados

## 📋 Menu do Sistema

Ao executar o programa, o seguinte menu é exibido no console:

=== Folha de pagamento ===  
1. Cadastrar funcionario padrão  
2. Cadastrar funcionario comissionado  
3. Cadastrar funcionario produção  
4. Gerar folha de pagamento  
0. Sair do programa  

## ▶ Como Executar o Projeto

Pré-requisitos:
- Java JDK 8 ou superior instalado

Passos:
1. Compile o arquivo:
   javac FolhaDePagamento.java

2. Execute o programa:
   java FolhaDePagamento

3. Utilize o menu interativo para cadastrar funcionários e gerar a folha de pagamento.

## 📤 Saída do Sistema

Ao gerar a folha de pagamento, o sistema exibe para cada funcionário:
- Nome
- Tipo de funcionário
- Matrícula
- Salário calculado

Também é exibida a quantidade total de funcionários cadastrados no sistema.

## 🎯 Objetivo do Projeto

Projeto desenvolvido com finalidade educacional para praticar conceitos de:
- Classes abstratas
- Herança
- Polimorfismo
- Estruturas de repetição
- Entrada de dados via console em Java

## 👨‍💻 Autor

Projeto acadêmico desenvolvido para estudo da linguagem Java e Programação Orientada a Objetos.
``
