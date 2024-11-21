print("Macuixtle Velazquez David\n")
class colors:
        HEADER = '\033[95m'
        OKBLUE = '\033[94m'
        OKCYAN = '\033[96m'
        OKGREEN = '\033[92m'
        WARNING = '\033[93m'
        FAIL = '\033[91m'
        
        BOLD = '\033[1m'
        UNDERLINE = '\033[4m'
        
        ENDC = '\033[0m'

class Cuenta(): 
    def __init__(self, num1, num2):
        self._num1=num1
        self._num2=num2

    def suma(self):
        resultado=self._num1 + self._num2
        print(f"El resultado de la suma es: {self._num1} + {self._num2}={resultado}")
    def resta(self):
        resultado=self._num1 - self._num2
        print(f"El resultado de la resta es: {self._num2} - {self._num1}={resultado}")
        if resultado <=-1:
            print(colors.FAIL+"**CUIDADO. TUS CUENTA ESTA EN NEGATIVO**"+ colors.ENDC)

class Años():
    def TitularValido(self,edad):
        self.edad=edad

print ("Cual es su edad?")
res1= int(input(": "))
if res1 >=18:
    print("Es valido")
else:
    print("No es valido")



print ("usted tiene 500 pesos en el banco\nDesea ingresaro retirar?")
res = int(input("1-Ingresar\n2-Retirar\n: "))
if res == 1:
    num1 = int(input("Ingrese la cantidad de dinero que desea ingresar: "))
    operacion=Cuenta(num1, 500) 
    operacion.suma()
else:
    num1 = int(input("Ingrese la cantidad de dinero que desea retirar: "))
    operacion=Cuenta(500,num1)
    operacion.resta()
![image](https://github.com/user-attachments/assets/cde4240a-7b58-48f5-b78e-4f3d8d7bd27a)
![image](https://github.com/user-attachments/assets/3a76c44f-0671-4f9c-b90b-21c2d46a9158)
