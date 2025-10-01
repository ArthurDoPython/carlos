1.
n1 = float(input("Digite o primeiro número: "))
n2 = float(input("Digite o segundo número: "))
print(f"Maior: {max(n1, n2)}")

2.
valor = float(input("Digite um valor: "))
if valor >= 0:
    print("Positivo")
else:
    print("Negativo")

3.
sexo = input("Digite F ou M: ").upper()
if sexo == 'F':
    print("F - Feminino")
elif sexo == 'M':
    print("M - Masculino")
else:
    print("Sexo Inválido")

4.
letra = input("Digite uma letra: ").upper()
if letra in 'AEIOU':
    print("Vogal")
else:
    print("Consoante")

5.
nota1 = float(input("Primeira nota: "))
nota2 = float(input("Segunda nota: "))
media = (nota1 + nota2) / 2
if media == 10:
    print("Aprovado com Distinção")
elif media >= 7:
    print("Aprovado")
else:
    print("Reprovado")

6.
n1 = float(input("Primeiro número: "))
n2 = float(input("Segundo número: "))
n3 = float(input("Terceiro número: "))
print(f"Maior: {max(n1, n2, n3)}")

7.
n1 = float(input("Primeiro número: "))
n2 = float(input("Segundo número: "))
n3 = float(input("Terceiro número: "))
print(f"Maior: {max(n1, n2, n3)}")
print(f"Menor: {min(n1, n2, n3)}")

8.
p1 = float(input("Preço do primeiro produto: "))
p2 = float(input("Preço do segundo produto: "))
p3 = float(input("Preço do terceiro produto: "))
print(f"Compre o produto de R$ {min(p1, p2, p3):.2f}")

9.
n1 = float(input("Primeiro número: "))
n2 = float(input("Segundo número: "))
n3 = float(input("Terceiro número: "))
numeros = [n1, n2, n3]
numeros.sort(reverse=True)
print(numeros)

10.
turno = input("Turno (M-matutino, V-vespertino, N-noturno): ").upper()
if turno == 'M':
    print("Bom Dia!")
elif turno == 'V':
    print("Boa Tarde!")
elif turno == 'N':
    print("Boa Noite!")
else:
    print("Valor Inválido!")

11.
salario = float(input("Salário: "))
if salario <= 280:
    percentual = 20
elif salario <= 700:
    percentual = 15
elif salario <= 1500:
    percentual = 10
else:
    percentual = 5
aumento = salario * percentual / 100
novo_salario = salario + aumento
print(f"Salário antes: R$ {salario:.2f}")
print(f"Percentual: {percentual}%")
print(f"Aumento: R$ {aumento:.2f}")
print(f"Novo salário: R$ {novo_salario:.2f}")

12.
valor_hora = float(input("Valor da hora: "))
horas = float(input("Horas trabalhadas: "))
salario_bruto = valor_hora * horas
if salario_bruto <= 900:
    ir = 0
elif salario_bruto <= 1500:
    ir = 5
elif salario_bruto <= 2500:
    ir = 10
else:
    ir = 20
desconto_ir = salario_bruto * (ir / 
