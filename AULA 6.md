1 - 
![image](https://github.com/user-attachments/assets/315016fc-3431-432a-9a63-cd0ffe905c8b)

2 - def calcular():
    # Solicita ao usuário o primeiro número
    num1 = float(input("Digite o primeiro número: "))
    
    # Solicita ao usuário o segundo número
    num2 = float(input("Digite o segundo número: "))
    
    # Solicita ao usuário a operação desejada
    operacao = input("Digite a operação desejada (+, -, *, /): ")
    
    # Calcula e imprime o resultado com base na operação escolhida
    if operacao == '+':
        resultado = num1 + num2
        print(f"Resultado: {num1} + {num2} = {resultado}")
    elif operacao == '-':
        resultado = num1 - num2
        print(f"Resultado: {num1} - {num2} = {resultado}")
    elif operacao == '*':
        resultado = num1 * num2
        print(f"Resultado: {num1} * {num2} = {resultado}")
    elif operacao == '/':
        if num2 != 0:
            resultado = num1 / num2
            print(f"Resultado: {num1} / {num2} = {resultado}")
        else:
            print("Erro: Divisão por zero não é permitida.")
    else:
        print("Operação inválida. Por favor, escolha +, -, * ou /.")

# Chama a função para executar
calcular()

código executado:
![image](https://github.com/user-attachments/assets/7415acc4-b665-4d65-b189-51d6df58586b)
