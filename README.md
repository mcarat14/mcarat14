import turtle

# Classe base Forma
class Forma:
    def desenhar(self):
        raise NotImplementedError("Este método deve ser sobrescrito na subclasse.")

# Subclasse Círculo
class Circulo(Forma):
    def __init__(self, raio):
        self.raio = raio

    def desenhar(self):
        t = turtle.Turtle()
        t.circle(self.raio)
        turtle.done()

# Subclasse Quadrado
class Quadrado(Forma):
    def __init__(self, lado):
        self.lado = lado

    def desenhar(self):
        t = turtle.Turtle()
        for _ in range(4):
            t.forward(self.l
