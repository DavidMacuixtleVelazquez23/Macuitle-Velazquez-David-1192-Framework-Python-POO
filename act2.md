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

![image](https://github.com/user-attachments/assets/85b047bd-ebec-423f-bca2-272a1894eebf)
![image](https://github.com/user-attachments/assets/70e95a7e-050d-47cd-90e5-a910c763e1a3)
