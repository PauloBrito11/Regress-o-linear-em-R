# Objetivo

O objetivo é encontrar uma correlação entre as variáveis que nos permita realizar previsões.


## Contexto e inspeção inicial

Primeiramente, o conjunto de dados utilizado chama-se "Cars", contendo duas variáveis, são elas: velocidade e distância de freagem. Para verificar as características do conjunto de dados, utilizamos funções bem simples:

```r
head(cars)
colnames(cars)
```

Cinco primeiras linhas:

![image](https://github.com/user-attachments/assets/c163d724-c5c6-4726-9e51-a354b58feed4)

Nome das colunas (variáveis):

![image](https://github.com/user-attachments/assets/22e3e4d8-5c75-42ae-b001-c914a6a39098)

## Iniciando o processo

Verificando a correlação entre as varíaveis:

```r
cor(cars)
```

Resultado:

![image](https://github.com/user-attachments/assets/5bac00b8-12a2-4f64-a8f1-ed2ee268313f)


É importante ressaltar que  a função retorna uma matriz de ordem 2, portanto, possuimos quatro resultados, entretanto, as variáveis se correlacionam com si mesmas, então o resultado de duas colunas é o valor 1, e o resultado das outras duas é a "verdadeira correlação".

Criando o modelo:

```r
modelo = lm(speed ~ dist, data=cars)

#a função "LM", recebe dois parâmetros: ("formula", "data")
```




