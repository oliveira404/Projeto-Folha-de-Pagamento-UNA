# Folha de Pagamento em Java

Projeto desenvolvido em Java que simula uma **folha de pagamento**, permitindo o cadastro de diferentes tipos de funcionários e o cálculo automático de seus salários, de acordo com regras específicas.

O sistema funciona via **terminal** e utiliza conceitos fundamentais da **Programação Orientada a Objetos (POO)**.

---

## 📌 Objetivo do Projeto

O objetivo deste projeto é aplicar, na prática, os principais conceitos de Java e POO, como:

- Classes abstratas
- Herança
- Polimorfismo
- Organização de classes
- Uso de listas dinâmicas
- Entrada de dados via terminal

---

## ⚙️ Funcionalidades

- Menu interativo no terminal
- Cadastro de funcionários
- Cálculo automático de salários
- Armazenamento dos funcionários em lista
- Exibição de todos os funcionários cadastrados ao encerrar o programa

---

## 🧱 Tipos de Funcionários

### 👤 Funcionário Padrão
- Possui salário fixo.

### 💰 Funcionário Comissionado
- Salário fixo
- Acréscimo baseado em:
  - Valor das vendas
  - Percentual de comissão

### 🏭 Funcionário de Produção
- Salário fixo
- Acréscimo proporcional à:
  - Quantidade de peças produzidas
  - Valor de cada peça

---

## 🧠 Estrutura do Projeto

O programa é composto pelas seguintes classes:

- `Funcionario` (classe abstrata)
- `FuncionarioPadrao`
- `FuncionarioComissionado`
- `FuncionarioProducao`
- `FolhaDePagamento` (classe principal com `main`)

Todas as classes estão implementadas em um único arquivo para facilitar o estudo e a execução.

---

## 🛠️ Tecnologias Utilizadas

- Java (JDK 8 ou superior)
- `Scanner` para entrada de dados
- `ArrayList` para armazenamento dinâmico

---

## ▶️ Como Executar o Projeto

### Pré-requisitos
- Java instalado na máquina

Verifique com:
```bash
java -version
