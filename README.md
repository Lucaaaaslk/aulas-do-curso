class Carro:
    def __init__(self, marca, modelo, cor, ano, valor):
        self.marca = marca
        self.modelo = modelo
        self.cor = cor
        self.ano = ano
        self.valor = valor

class Estoque:
    def __init__(self):
        self.carro = []  #

    def adicionar_carro(self, carro):
        self.carro.append(carro)  

    def Mostra_Estoque(self):
        for carro in self.carro:  
            print(f'{carro.modelo}, {carro.marca}')

carro_1 = Carro('porche', '911', 'verde', '1999', 1000000)
carro_2 = Carro('Honda', 'civic', 'branco', '2000', 250000)
carro_3 = Carro('toyota', 'corolla', 'vermelho', '2005', 150000)

estoque = Estoque()
estoque.adicionar_carro(carro_1)
estoque.adicionar_carro(carro_2)  # Adicionando mais carros para testar
estoque.adicionar_carro(carro_3)

estoque.Mostra_Estoque()
