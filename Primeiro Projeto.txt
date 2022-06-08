#Calculadora de equação de segundo grau

###Entrada de dados
A = int(input('valor de A: '))
B = int(input('valor de B: '))
C = int(input('valor de C: '))
Delta = (B**2)-4*(A*C)
print('valor de delta',Delta)
###Condicionando saída de dados
if Delta < 0:
  print('Não há solução real')
elif Delta == 0:
  print('Há duas raízes iguais e reais.')
  X1 = -(B)/(2*A)
  X2 = -(B)/(2*A)
  print(f'Primeira raíz = {X1}') 
  print(f'Segunda raíz = {X2}')
elif Delta > 0:
  print('Há duas raízes iguais e diferentes.')
  X1 = (-B+Delta**0.5)/2*A
  X2 = (-B-Delta**0.5)/2*A
  print(f'Primeira raíz = {X1}') 
  print(f'Segunda raíz = {X2}')
else:
  print('erro')