#Relatório do TP2
##Data:2024/09/22
##Autor:Pedro Oliveira a100625
 ##TPC
 
 from random import randint
 numerocomputador=randint(0,100)
 print("Ola..eu sou o computador e acabei de pensar num numero entre 0 e 100")
 print("Tenta adivinhar o numero com o menor numero de tenativas possiveis")

 numeroutilizador=int(input("Introduz o teu palpite"))
 contadortentativas=1
 while numeroutilizador != numerocomputador:
    if numeroutilizador > numerocomputador:
      print("O numero que pensei é menor")
    elif numeroutilizador < numerocomputador:
       print("O numero que pensei é maior")
    numeroutilizador=int(input("Tente novamente"))
    contadortentativas +=1
 print(f"Parabens..Acertou com {contadortentativas} tentativas..")
