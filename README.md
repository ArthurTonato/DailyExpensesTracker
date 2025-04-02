# Daily Expense Tracker

## ✨ Introdução
O **Daily Expense Tracker** é um programa simples em Python para ajudar os usuários a registrar e gerenciar seus gastos diários. Com ele, é possível adicionar despesas, visualizar todas as entradas, calcular o total e a média dos gastos, limpar o histórico e sair do programa.

---

## 🔮 Índice
1. [Recursos](#-recursos)
2. [Tecnologias Utilizadas](#-tecnologias-utilizadas)
3. [Como Clonar o Repositório](#-como-clonar-o-repositório)
4. [Como Executar o Programa](#-como-executar-o-programa)
5. [Explicação do Código](#-explicação-do-código)
6. [Glossário](#-glossário)
7. [Contribuição](#-contribuição)

---

## ⚙️ Recursos
- Adicionar uma nova despesa
- Visualizar todas as despesas registradas
- Calcular o total e a média das despesas
- Limpar todas as despesas
- Sair do programa

---

## 💻 Tecnologias Utilizadas
- **Linguagem:** Python 3+

---

## 📚 Como Clonar o Repositório
Para copiar o projeto para sua máquina local, utilize o seguinte comando:
```bash
git clone https://github.com/seu-usuario/daily-expense-tracker.git
```

Depois, acesse o diretório do projeto:
```bash
cd daily-expense-tracker
```

---

## 🚀 Como Executar o Programa
1. Certifique-se de ter o Python instalado na sua máquina.
2. No terminal, navegue até a pasta do projeto.
3. Execute o programa com o seguinte comando:
   ```bash
   python daily_expense_tracker.py
   ```
4. Utilize o menu para interagir com o sistema.

---

## 🔍 Explicação do Código
### 1. Exibição do Menu Inicial
```python
print("Welcome to the Daily Expense Tracker!")

print("\nMenu:")
print("1. Add a new expense")
print("2. View all expenses")
print("3. Calculate total and average expense")
print("4. Clear all expenses")
print("5. Exit")
```
- Exibe a mensagem de boas-vindas e o menu de opções para o usuário.

### 2. Lista de Despesas
```python
expenses = []
```
- Cria uma lista vazia para armazenar as despesas.

### 3. Loop Principal
```python
while True:
```
- Mantém o programa em execução até que o usuário escolha sair.

### 4. Captura de Entrada do Usuário
```python
choice = input()
```
- Solicita ao usuário uma escolha do menu.

### 5. Opções do Menu
- **Adicionar despesa**
  ```python
  amount = float(input())
  expenses.append(amount)
  print("Expense added successfully!")
  ```
  - O programa solicita um valor, adiciona à lista e confirma a inclusão.

- **Exibir todas as despesas**
  ```python
  if expenses == []:
      print("No expenses recorded yet.")
  else:
      print("Your expenses:")
      for i in range(len(expenses)):
          print(f"{i+1}.", expenses[i])
  ```
  - Se houver despesas, elas são exibidas na tela.

- **Calcular total e média**
  ```python
  if expenses == []:
      print("No expenses recorded yet.")
  else:
      new_exp = sum(expenses)
      avg = new_exp / len(expenses)
      print(f"Total expense: {new_exp}")
      print(f"Average expense: {avg}")
  ```
  - O programa calcula a soma e a média dos valores registrados.

- **Limpar todas as despesas**
  ```python
  expenses.clear()
  print("All expenses cleared.")
  ```
  - Remove todas as despesas da lista.

- **Sair do programa**
  ```python
  print("Exiting the Daily Expense Tracker. Goodbye!")
  break
  ```
  - Exibe uma mensagem de despedida e encerra o loop.

- **Entrada Inválida**
  ```python
  else:
      print("Invalid choice. Please try again.")
  ```
  - Informa ao usuário que a entrada é inválida.

---

## 🤖 Glossário
| Termo         | Definição |
|--------------|------------|
| `input()`    | Função do Python usada para capturar entrada do usuário |
| `float()`    | Converte um valor para um número decimal |
| `append()`   | Adiciona um elemento a uma lista |
| `sum()`      | Retorna a soma de todos os elementos de uma lista |
| `clear()`    | Remove todos os elementos de uma lista |
| `break`      | Interrompe a execução de um loop |

---

## 📝 Contribuição
Se você quiser contribuir com melhorias para o **Daily Expense Tracker**, siga estes passos:
1. Faça um fork do repositório.
2. Crie uma branch para sua feature:
   ```bash
   git checkout -b minha-feature
   ```
3. Faça suas alterações e commit:
   ```bash
   git commit -m "Adicionando nova funcionalidade"
   ```
4. Envie suas alterações:
   ```bash
   git push origin minha-feature
   ```
5. Abra um **Pull Request** no GitHub.

---

## 🚀 Pronto para começar?
Baixe o repositório e comece a rastrear suas despesas agora mesmo! 🙌

