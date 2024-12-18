# Desafio-Dificil-ProZ-Educacao
Crie uma função para pedir um numero divisivel por 2 e por 3, com mensagens de erro apropriados para cada cenario possivel.

def par():
  print("Escreva um número par:")
  eh_par = False
  while(eh_par == False):
    try:
      num_par = int(input())
      if (num_par % 2 != 0):
        print(str(num_par), "é um número ímpar. Por favor digite um número par")
      elif ((num_par % 2 != 0) or (num_par % 3 != 0)):
        print("O número precisa ser um divisível por 2 e 3")
      else:
        print("Obrigado! O número digitado é: " + str(num_par))
        eh_par = True
    except:
      print("Você precisa digitar um número inteiro!")

par()
