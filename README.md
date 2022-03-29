
#Simulador de dado
# Simular o uso de um dado, gerando uma valor de 1 ate 6
from logging import exception
import random
import PySimpleGUI

class SimuladorDeDado:
    def __init__(self):
        self.valor_minimo = 1
        self.valor_maximo = 6
        self.mensagem = 'Voce gostaria de gerar um novo valor para o dado ?'
        #layout
        layout = [
            [sg.]
        ]
        #criar uma janela
        #ler os valores da tela
        #Fazer alguma coisa com esses valores 

    def Iniciar(self):
        reposta = input(self.mensagem)
        try:
            if reposta == 'sim' or reposta == 's':
                self.GerarValordoDado()
            elif reposta == 'não' or reposta == 'n':
                print ('Agradecemos sua participaçao!')
            else:
                print('Favor digitar sim ou não')
        except:
                print('Ocorreu um erro ao receber sua resposta')
                

    def GerarValordoDado(self):
        print(random.randint(self.valor_minimo, self.valor_maximo))



simulador = SimuladorDeDado()
simulador.Iniciar()
