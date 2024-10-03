#Desafio funções pela DIO. 
#Linguagem escolhida: Python
#Autor: kimijima1

def saldoDeVitorias(v,d):
    if (v-d)<10:
        return (v-d)
    elif 11<(v-d)<20:
        return (v-d)
    elif 21<(v-d)<50:
        return (v-d)
    elif 51<(v-d)<80:
        return (v-d)
    elif 81<(v-d)<90:
        return (v-d)
    elif 91<(v-d)<100:
        return (v-d)
    else:
        return (v-d)
def rank(v,d):
    if (v-d)<10:
        return "ferro"
    elif 11<(v-d)<20:
        return bronze
    elif 21<(v-d)<50:
        return "prata"
    elif 51<(v-d)<80:
        return "ouro"
    elif 81<(v-d)<90:
        return "diamante"
    elif 91<(v-d)<100:
        return "imortal"
    else:
        return "lendario"
v=int(input("Qual é a quantidade de vitórias? "))
d=int(input("Qual é a quantidade de derrotas? "))
saldoTotal=saldoDeVitorias(v,d)
ranking=rank(v,d)
print(f"Seu saldo de vitórias é de: {saldoTotal} e seu ranking é: {ranking}")
