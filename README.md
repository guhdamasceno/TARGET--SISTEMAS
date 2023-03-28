'''Dado a sequência de Fibonacci, onde se inicia por 0 e 1 e o próximo valor sempre será a soma dos 2 valores anteriores
(exemplo: 0, 1, 1, 2, 3, 5, 8, 13, 21, 34...), escreva um programa na linguagem que desejar onde,
informado um número, ele calcule a sequência de Fibonacci e retorne uma mensagem avisando se o número informado pertence ou não a sequência.'''


termo1 = int(0)
termo2 = int(1)
termo3 = int(0)
valor = int(input('Digite um número: '))
while valor > termo3:
    termo3 = termo1 + termo2
    termo1 = termo2
    termo2 = termo3
if valor == 0 or valor == 1:
    print ('O número faz parte da sequência de Fibonacci.')
elif valor == termo3:
    print ('O número faz parte da sequência de Fibonacci.')
else:
    print ('O número digitado não faz parte da sequência de Fibonacci.')
    
    
    
    
    ) Dado um vetor que guarda o valor de faturamento diário de uma distribuidora, faça um programa, na linguagem que desejar, que calcule e retorne:
    
• O menor valor de faturamento ocorrido em um dia do mês;
• O maior valor de faturamento ocorrido em um dia do mês;
• Número de dias no mês em que o valor de faturamento diário foi superior à média mensal.'''

soma = 0
total = 0
maior = menor = 0
superior = 0
dia = 0
while True:
    dia +=1
    num = float(input(f'Digite o valor do faturamento do dia {dia} : R$'))
    total +=1
    soma += num
    media = soma / total
    if total == 1:
        maior = num
        menor = num
    else:
        if num > maior:
            maior = num
        if num < menor:
            menor = num
    if maior > media:
        superior += 1

    if dia == 30:
        break

print(f'O maior valor de faturamento em um dia foi R${maior}')
print(f'O menor valor de faturamento em um dia foi R${menor}')
print(f'Em {superior} dias o faturamento foi acima da media.')








'''Dado o valor de faturamento mensal de uma distribuidora, detalhado por estado:

SP – R$67.836,43
RJ – R$36.678,66
MG – R$29.229,88
ES – R$27.165,48
Outros – R$19.849,53'''

sp = float(67.83643)
rj = float(36.67866)
mg = float(29.22988)
es = float(27.16548)
out = float(19.84953)
total = float(sp + rj + mg + es + out)
print(total)
psp = ((sp*total)/100)
prj = ((rj*total)/100)
pmg = ((mg*total)/100)
pes = ((es*total)/100)
pout = ((out*total)/100)

print('Porcentagem de SP {}'.format(psp))
print('Porcentagem de RJ {}'.format(prj))
print('Porcentagem de MG {}'.format(pmg))
print('Porcentagem de ES {}'.format(pes))
print('Porcentagem de OUT {}'.format(pout))









'''Escreva um programa que inverta os caracteres de um string'''


txt = input('Digite um texto para inverter: ')
print (txt[::-1])
