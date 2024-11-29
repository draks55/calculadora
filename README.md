# Menú de la calculadora
print("=== Calculadora Básica ===")
print("1. Sumar")
print("2. Restar")
print("3. Multiplicar")
print("4. Dividir")

# Pedir al usuario que elija una operación
opcion = int(input("Elige una opción (1-4): "))

# Pedir dos números al usuario
num1 = float(input("Ingresa el primer número: "))
num2 = float(input("Ingresa el segundo número: "))

# Realizar la operación según la opción elegida
if opcion == 1:
    resultado = num1 + num2
    print("El resultado de la suma es:", resultado)
elif opcion == 2:
    resultado = num1 - num2
    print("El resultado de la resta es:", resultado)
elif opcion == 3:
    resultado = num1 * num2
    print("El resultado de la multiplicación es:", resultado)
elif opcion == 4:
    if num2 != 0:
        resultado = num1 / num2
        print("El resultado de la división es:", resultado)
    else:
        print("Error: No se puede dividir entre cero.")
else:
    print("Opción inválida. Por favor, elige entre 1 y 4.")
