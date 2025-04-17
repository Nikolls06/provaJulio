# provaJulio

1
uso_cpu = [
[20, 25, 40, 50, 45, 60, 55, 35, 70, 65],
[30, 35, 50, 60, 40, 55, 60, 45, 50, 55],
[15, 20, 30, 25, 35, 40, 45, 50, 55, 60],
[10, 15, 25, 35, 45, 50, 55, 60, 65, 70],
]

for linha in uso_cpu:
    media = sum(linha) / len(linha)
    print("Média de uso CPU é: ",media)

2
def alerta_uso():
    for lista in uso_cpu:
        for i in lista:
            if i > 85:
                print("True")
            else:
                print("False")
alerta_uso()

3
def dados_crescente():
    for i in uso_cpu:
            i.sort()
            print(i)
dados_crescente()


PANDAS

import pandas as pd
uso_cpu = [
[20, 25, 40, 50, 45, 60, 55, 35, 70, 65],
[30, 35, 50, 60, 40, 55, 60, 45, 50, 55],
[15, 20, 30, 25, 35, 40, 45, 50, 55, 60],
[10, 15, 25, 35, 45, 50, 55, 60, 65, 70],
]
df = pd.DataFrame(uso_cpu)

df.columns = ['1h', '2h', '3h', '4h', '5h', '6h', '7h', '8h', '9h', '10h']

df
