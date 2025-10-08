# 🧩 Projeto IMC – Calculadora de Índice de Massa Corporal

## 🎯 Objetivo do Exercício
Crie um aplicativo usando **Flet** que calcule o **IMC (Índice de Massa Corporal)** de uma pessoa.  
O app deve permitir que o usuário digite o **peso (kg)** e a **altura (m)**, e ao clicar em um botão, exiba o resultado por meio de um **`snackbar`**.

---

## 🧠 Instruções para os alunos
1. Crie um arquivo chamado **`projeto_imc.py`**.  
2. Importe o módulo **Flet**.  
3. Crie campos para digitar:
   - Peso
   - Altura
4. Crie um botão chamado **“Calcular IMC”**.  
5. Ao clicar, o sistema deve calcular o IMC usando a fórmula:
   ```python
   IMC = peso / (altura * altura)
   ```
6. Mostre o resultado em um **`snackbar`**, com uma mensagem informando a **classificação** do IMC:
   - Abaixo do peso: IMC < 18.5  
   - Peso normal: 18.5 ≤ IMC < 24.9  
   - Sobrepeso: 25 ≤ IMC < 29.9  
   - Obesidade: IMC ≥ 30  

---
7. Exemplo de como deve ficar ( pode melhor a interface se conseguir!!! )
<img width="589" height="598" alt="image" src="https://github.com/user-attachments/assets/91c7b3b4-64b2-44a7-ab6f-78876bd39940" />

## ✅ Código para completar
```python
import flet as ft

def main(page: ft.Page):
    page.title = "Projeto IMC"
    page.theme_mode = "light" # dark
    page.vertical_alignment = "center"
    page.horizontal_alignment = "center"
    page.window.width = 600
    page.window.height = 600


    # Título
    ...

    # Campos de entrada
    ...

    # Função para calcular o IMC
    def calcular_imc(e):


    # Botão de ação

    # Adicionando elementos à página
    page.add(
        titulo,
        peso,
        altura,
        botao
    )

ft.app(target=main)
```

---

## 🧾 Explicação Rápida
- `snack_bar`: exibe uma notificação temporária na parte inferior da tela.  
- `try/except`: garante que o programa não trave se o aluno digitar letras ou deixar campos vazios.  
- `page.update()`: atualiza a interface após abrir o snackbar.  

