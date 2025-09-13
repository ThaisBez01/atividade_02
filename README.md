#Crie um programa em python que calcule o IMC do usuário. O programa irá informar o valor do IMC e informar o diagnóstico (consultar a tabela do IMC na internet)

# Solicitar dados ao usuário
peso = float(input("Informe seu peso em kg: "))
altura = float(input("Informe sua altura em metros: "))


imc = peso / (altura ** 2)


print(f"\nSeu IMC é: {imc:.2f}")


if imc < 18.5:
    resultado = "Abaixo do peso"
elif 18.5 <= imc < 24.9:
    resultado = "Peso normal"
elif 25 <= imc < 29.9:
    resultado = "Sobrepeso"
elif 30 <= imc < 34.9:
    resultado = "Obesidade grau 1"
elif 35 <= imc < 39.9:
    resultado = "Obesidade grau 2"
else:
    resultado = "Obesidade grau 3"

# Exibir o diagnóstico
print(f"Resultado: {resultado}")
