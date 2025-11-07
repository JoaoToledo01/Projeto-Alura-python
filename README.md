# Projeto-Alura-python
# Programa para verificar a organização do evento da escola

# Leitura dos dados de entrada
alunos = int(input("Digite a quantidade de alunos: "))
monitores = int(input("Digite a quantidade de monitores: "))
convidados = int(input("Digite a quantidade de convidados: "))

# Cálculo do total de pessoas
total_pessoas = alunos + monitores + convidados

# Verificações de regras
if total_pessoas > 100:
    print("\n❌ Não é possível acomodar todas as pessoas.")
    print(f"O total de {total_pessoas} excede os 100 ingressos disponíveis.")
elif convidados > 20:
    print("\n⚠️ Número de convidados excede o limite permitido.")
    print(f"Foram informados {convidados} convidados, mas o máximo é 20.")
else:
    print("\n✅ Tudo certo! O evento pode ser organizado dentro das regras.")
    print(f"Total de pessoas: {total_pessoas}")
    print(f"Convidados: {convidados}")
