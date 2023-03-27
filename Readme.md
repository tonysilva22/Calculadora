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




# Função principal da calculadora

def calculadora():
    operacoes = {
        "+": soma,
        "-": subtracao,
        "*": multiplicacao,
        "/": divisao
    }

    while True:





 # Solicita a operação e os dois números para o usuário
        operacao = input("Digite a operação (+, -, *, /): ")
        if operacao not in operacoes:
            print("Operação inválida!")
            continue
        num1 = float(input("Digite o primeiro número: "))
        num2 = float(input("Digite o segundo número: "))
        
        
 # Chama a função correspondente à operação solicitada
        resultado = operacoes[operacao](num1, num2)
        print("Resultado: ", resultado)
        
        
        
  # Pergunta ao usuário se deseja continuar calculando
        continuar = input("Deseja continuar calculando? (S/N): ")
        if continuar.lower() != "s":
            break


# Chama a função principal da calculadora
calculadora()
        
        
        
        
        
        
        
        
   
