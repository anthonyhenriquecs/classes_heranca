# classes_heranca


class Veiculo:
    def __init__(self, cor, placa, numero_rodas):
        self.cor = cor
        self.placa = placa
        self.numero_rodas = numero_rodas

    def ligar_motor(self):
        print("ligando o motor...")
class Motomoto(Veiculo):
    pass
class Carro(Veiculo):
    pass
class Caminhão(Veiculo):
    def __init__(self,carregado,cor, placa, numero_rodas):
        self.carregado = carregado
    def esta_carregado(self):
        self.r = input("ESTA CARREGADO? ")
        if self.r == "s":
            print("Pronto pra partir")
        else:   
            print("não estou carregado...")


moto = Motomoto("preta","adb",2)
moto.ligar_motor()

carro = Carro("corola", "123-abc", 4)
carro.ligar_motor()

caminhao = Caminhão("v8", "321-cba",8,True)
caminhao.esta_carregado()
