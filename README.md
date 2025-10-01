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
desconto_ir = salario_bruto * (ir / 100)
inss = salario_bruto * 0.10
fgts = salario_bruto * 0.11
total_descontos = desconto_ir + inss
salario_liquido = salario_bruto - total_descontos
print(f"Salário Bruto: R$ {salario_bruto:.2f}")
print(f"(-) IR ({ir}%): R$ {desconto_ir:.2f}")
print(f"(-) INSS (10%): R$ {inss:.2f}")
print(f"FGTS (11%): R$ {fgts:.2f}")
print(f"Total descontos: R$ {total_descontos:.2f}")
print(f"Salário Líquido: R$ {salario_liquido:.2f}")

13.
dia = int(input("Número (1-7): "))
dias = {1: "Domingo", 2: "Segunda", 3: "Terça", 4: "Quarta", 5: "Quinta", 6: "Sexta", 7: "Sábado"}
print(dias.get(dia, "Valor inválido"))

14.
nota1 = float(input("Primeira nota: "))
nota2 = float(input("Segunda nota: "))
media = (nota1 + nota2) / 2
if media >= 9:
    conceito = 'A'
elif media >= 7.5:
    conceito = 'B'
elif media >= 6:
    conceito = 'C'
elif media >= 4:
    conceito = 'D'
else:
    conceito = 'E'
print(f"Média: {media:.2f}")
print(f"Conceito: {conceito}")

15.
l1 = float(input("Lado 1: "))
l2 = float(input("Lado 2: "))
l3 = float(input("Lado 3: "))
if l1 + l2 > l3 and l1 + l3 > l2 and l2 + l3 > l1:
    if l1 == l2 == l3:
        print("Equilátero")
    elif l1 == l2 or l1 == l3 or l2 == l3:
        print("Isósceles")
    else:
        print("Escaleno")
else:
    print("Não forma triângulo")

16.
a = float(input("a: "))
if a == 0:
    print("Não é equação do segundo grau")
else:
    b = float(input("b: "))
    c = float(input("c: "))
    delta = b**2 - 4*a*c
    if delta < 0:
        print("Não possui raízes reais")
    elif delta == 0:
        raiz = -b / (2*a)
        print(f"Raiz única: {raiz}")
    else:
        raiz1 = (-b + delta**0.5) / (2*a)
        raiz2 = (-b - delta**0.5) / (2*a)
        print(f"Raízes: {raiz1} e {raiz2}")

17.
ano = int(input("Ano: "))
if (ano % 4 == 0 and ano % 100 != 0) or (ano % 400 == 0):
    print("Bissexto")
else:
    print("Não é bissexto")

18.
data = input("Data (dd/mm/aaaa): ")
dia, mes, ano = map(int, data.split('/'))
valida = False
if mes in [1, 3, 5, 7, 8, 10, 12]:
    if 1 <= dia <= 31:
        valida = True
elif mes in [4, 6, 9, 11]:
    if 1 <= dia <= 30:
        valida = True
elif mes == 2:
    if (ano % 4 == 0 and ano % 100 != 0) or (ano % 400 == 0):
        if 1 <= dia <= 29:
            valida = True
    else:
        if 1 <= dia <= 28:
            valida = True
if valida:
    print("Data válida")
else:
    print("Data inválida")
