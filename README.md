# Upcasting e Downcasting em Java

Este repositório contém um exemplo em **Java** que demonstra os conceitos de **upcasting** e **downcasting** usando uma hierarquia de classes de contas bancárias.

---

## 📁 Estrutura do Projeto

```text
src/
├── application/
│   └── Program.java
└── entities/
    ├── Account.java
    ├── BusinessAccount.java
    └── SavingsAccount.java
```

---

## 📌 Descrição dos Arquivos

### `Program.java`

Classe principal do programa que demonstra o uso de upcasting e downcasting ao criar e manipular objetos das classes de conta.

### `Account.java`

Classe base que representa uma conta bancária com atributos e métodos comuns, como número da conta, titular e saldo.

### `BusinessAccount.java`

Classe que estende `Account`, representando uma conta empresarial com funcionalidades adicionais.

### `SavingsAccount.java`

Classe que estende `Account`, representando uma conta poupança com regras específicas.

---

## ⚙️ Conceitos de Java Utilizados

### 🔹 Herança

As classes `BusinessAccount` e `SavingsAccount` **herdam** de `Account`, permitindo compartilhar atributos e métodos comuns.
```java
public class BusinessAccount extends Account { ... }
public class SavingsAccount extends Account { ... }
````
### 🔹 Upcasting

Upcasting é a conversão de um objeto de uma subclasse para o tipo da superclasse. Isso é feito de forma implícita e permite tratar objetos específicos como genéricos.

```java
Account acc1 = new BusinessAccount(...);
````
### 🔹 Downcasting

Downcasting é a conversão de um objeto do tipo da superclasse para uma subclasse. Requer cast explícito e deve ser usado com cuidado.

```java
BusinessAccount bAcc = (BusinessAccount) acc1;
````
