# Adivina-Adivinador_TorresOlvera

Torres Olvera Gael

En esta actividad realizaremos un codigo que nos haga tener que adivinar un numero

#En esta actvididad realizaremos un codigo que nos haga intentar adivinar el numero

print (" ")
print ("Torres Olvera Gael")
print (" ")

import random

def adivina_el_numero():
    numero_secreto = random.randint(1, 100)
    intentos = 0
    adivinado = False

    print("¡Bienvenido al juego de Adivina el Número!")
    print("He elegido un número entre 1 y 100. ¡Intenta adivinarlo!")

    while not adivinado:
        try:
            # Pide al usuario que ingrese un número
            adivinanza = int(input("Introduce tu adivinanza: "))
            intentos += 1

            if adivinanza < numero_secreto:
                print("Demasiado bajo. Intenta de nuevo.")
            elif adivinanza > numero_secreto:
                print("Demasiado alto. Intenta de nuevo.")
            else:
                adivinado = True
                print(f"¡Felicidades! Has adivinado el número en {intentos} intentos.")
        except ValueError:
            print("Por favor, introduce un número válido.")

if __name__ == "__main__":
    adivina_el_numero()

![image](https://github.com/user-attachments/assets/c5a3fc98-0139-462c-b017-5bf95a6b3ff4)
![image](https://github.com/user-attachments/assets/8942bc08-884a-477e-b54e-a9f5b680b073)
