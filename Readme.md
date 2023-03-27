# Projeto Calculadora

Este código permite ao usuário escolher uma das quatro operações matemáticas básicas (+, -, *, /) e inserir dois números para serem calculados. O código também inclui verificação para evitar divisão por zero. O usuário pode continuar fazendo quantas vezes desejar, até decidir sair do programa

# Define uma função para cada operação matemática

def soma(num1, num2):
    return num1 + num2

def subtracao(num1, num2):
    return num1 - num2

def multiplicacao(num1, num2):
    return num1 * num2

def divisao(num1, num2):
    if num2 == 0:
        return "Erro: divisão por zero"
    else:
        return num1 / num2
