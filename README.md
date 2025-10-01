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

19.
numero = int(input("Número (0-999): "))
if numero < 0 or numero > 999:
    print("Número inválido")
else:
    centenas = numero // 100
    dezenas = (numero % 100) // 10
    unidades = numero % 10
    partes = []
    if centenas > 0:
        partes.append(f"{centenas} centena{'s' if centenas > 1 else ''}")
    if dezenas > 0:
        partes.append(f"{dezenas} dezena{'s' if dezenas > 1 else ''}")
    if unidades > 0:
        partes.append(f"{unidades} unidade{'s' if unidades > 1 else ''}")
    print(" e ".join(partes))

20.
nota1 = float(input("Primeira nota: "))
nota2 = float(input("Segunda nota: "))
nota3 = float(input("Terceira nota: "))
media = (nota1 + nota2 + nota3) / 3
if media == 10:
    print(f"Aprovado com Distinção - Média: {media:.2f}")
elif media >= 7:
    print(f"Aprovado - Média: {media:.2f}")
else:
    print(f"Reprovado - Média: {media:.2f}")

21.
valor = int(input("Valor do saque (10-600): "))
if valor < 10 or valor > 600:
    print("Valor inválido")
else:
    notas_100 = valor // 100
    valor %= 100
    notas_50 = valor // 50
    valor %= 50
    notas_10 = valor // 10
    valor %= 10
    notas_5 = valor // 5
    notas_1 = valor % 5
    if notas_100 > 0:
        print(f"{notas_100} nota(s) de 100")
    if notas_50 > 0:
        print(f"{notas_50} nota(s) de 50")
    if notas_10 > 0:
        print(f"{notas_10} nota(s) de 10")
    if notas_5 > 0:
        print(f"{notas_5} nota(s) de 5")
    if notas_1 > 0:
        print(f"{notas_1} nota(s) de 1")

22.
numero = int(input("Número: "))
if numero % 2 == 0:
    print("Par")
else:
    print("Ímpar")

23.
numero = float(input("Número: "))
if numero == int(numero):
    print("Inteiro")
else:
    print("Decimal")

24.
n1 = float(input("Primeiro número: "))
n2 = float(input("Segundo número: "))
operacao = input("Operação (+, -, *, /): ")
if operacao == '+':
    resultado = n1 + n2
elif operacao == '-':
    resultado = n1 - n2
elif operacao == '*':
    resultado = n1 * n2
elif operacao == '/':
    resultado = n1 / n2
else:
    print("Operação inválida")
    resultado = None
if resultado is not None:
    print(f"Resultado: {resultado}")
    print(f"Par" if resultado % 2 == 0 else "Ímpar")
    print(f"Positivo" if resultado >= 0 else "Negativo")
    print(f"Inteiro" if resultado == int(resultado) else "Decimal")

25.
respostas = []
respostas.append(input("Telefonou para a vítima? (s/n): ").lower())
respostas.append(input("Esteve no local do crime? (s/n): ").lower())
respostas.append(input("Mora perto da vítima? (s/n): ").lower())
respostas.append(input("Devia para a vítima? (s/n): ").lower())
respostas.append(input("Já trabalhou com a vítima? (s/n): ").lower())
positivas = respostas.count('s')
if positivas == 2:
    print("Suspeita")
elif 3 <= positivas <= 4:
    print("Cúmplice")
elif positivas == 5:
    print("Assassino")
else:
    print("Inocente")

26.
litros = float(input("Litros: "))
tipo = input("Tipo (A-álcool, G-gasolina): ").upper()
if tipo == 'A':
    preco = 1.90
    if litros <= 20:
        desconto = 0.03
    else:
        desconto = 0.05
elif tipo == 'G':
    preco = 2.50
    if litros <= 20:
        desconto = 0.04
    else:
        desconto = 0.06
else:
    print("Tipo inválido")
    desconto = 0
    preco = 0
total = litros * preco * (1 - desconto)
print(f"Total: R$ {total:.2f}")

27.
morangos = float(input("Kg de morangos: "))
macas = float(input("Kg de maçãs: "))
if morangos <= 5:
    preco_morango = 2.50
else:
    preco_morango = 2.20
if macas <= 5:
    preco_maca = 1.80
else:
    preco_maca = 1.50
total = (morangos * preco_morango) + (macas * preco_maca)
if morangos + macas > 8 or total > 25:
    total *= 0.9
print(f"Total: R$ {total:.2f}")
