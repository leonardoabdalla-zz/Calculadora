# Calculadora
Calculdora
entrada = input('Deseja utilizar a calculadora? (S/N) ')
while ( entrada == 'S'):
    entrada = input('Deseja realizar operação simples ou equação do segundo grau? (simples/equação) ')
    if entrada == 'equação':
        a = int(input('Digite numero de A(x2): '))
        b = int(input('Digite o numero de B(x): '))
        c = int(input('digite o numero de C:'))
        x1 = (-b + ((b ** 2 - 4 * a * c) ** 0.5)) / 2 * a
        x2 = (-b - ((b ** 2 - 4 * a * c) ** 0.5)) / 2 * a
        print(x1, x2)
    elif entrada == 'simples':
        numeroA = int(input('Digite o primeiro numero: '))
        operacao = input('Escolha  operação desejada(+ ; - ; / ; * ; %) :')
        numeroB = int(input('Digite mais um numero: '))
        if operacao == '+':
            print('Resultado da soma: ', numeroA + numeroB)
        elif operacao == '-':
            print('Resultado da subtração: ', numeroA - numeroB)
        elif operacao == '/':
            print('Resultado da divisão: ', numeroA / numeroB)
        elif operacao == '*':
            print('Resultado da multiplicação: ', numeroA * numeroB)
        elif operacao == '%':
            print(numeroA, 'porcentos de ', numeroB, 'é: ', numeroA*numeroB/100)
    else:
        print('esse operador não existe')
    entrada = input('Deseja realizar nova operação?(S/N) ')
print('Obrigado! Até a próxima')

