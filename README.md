# Taxa de transmissão de uma doença

## 1) Definição do problema: 

### Que problema estamos tentando resolver?  

Este case tem como objetivo avaliar os níveis de contaminação de um vírus no país X, gerando insights através de dados fornecidos pelo Gorverno.

![alt text](https://github.com/mcalmeida13/neoway-case/blob/main/img/2022-05-04_14-56.png?raw=true)




Sabe-se que a transmissão acontece de pessoa por pessoa, por isso elas devem estar conectadas de alguma maneira (familia, amizade ou trabalho). Foi fornecido um dataset com o nível de proximidade das pessoas e a frequência com que se encontram e a probabilidade da transmissão entre os indivíduos.

Já foi repassado também que a porbabilidade transmissão de um indivíduo A para B não é igual a de B para A, o que sugere que os atributos de cada indivíduo contribuem para a probabilidade de adoecer


![alt text](https://github.com/mcalmeida13/neoway-case/blob/main/img/2022-05-04_15-08.png?raw=true)

Foi fornecido outro dataset onde cada linha representa um indivíduo e um conjunto de atributos associados.

Machine learning pode ajudar com insights para:

1) saber quais features contribuem para a taxa de contaminação

2) prever a partir das features das duas pessoas a probabilidade de transmissão (Modelos de Regressão)

## 2) Dados:
Se o Machine learning está obtendo insights de dados, quais dados temos? Como ele corresponde à definição do problema? 
Dataset com cada entrada sendo as características dos usuários
Dataset de interação
Nossos dados são estruturados ou não estruturados? 
Estruturados
Estático ou streaming?
Estáticos

Para o desenvolvimentolução do problema considere os dois arquivos CSVo e res: 
#### `individuos_espec.csv`

características de cada indivíduo 
-`name`: Id dos indivíduos 
-`idade`: idade dos indivíduos 
-`estado_civil`: Estado civil dos indivíduos
-`qt_filhos`: quantidade de filhos dos indivíduos 
-`estuda`: caso estudem 
-`trabalha`: caso trabalhem 
-`pratica_esportes`: caso pratiquem esportes 
-`transporte_mais_utilizado`: qual o transporte mais utilizado 
-`IMC`: valor do índice de massa corporal dos indivíduos 

#### `conexoes_espec.csv` 

lista das conexões e algumas características das mesmas 
- `V1`: id do individuo (relação entre os indivíduos) 
- `V2`: id do individuo (relação entre os indivíduos) 
-`grau`: familia, amigos, trabalho 
-`proximidade`: 
    - mora_junto, 
    - visita_frequente, 
    - visita_casual, 
    - visita_rara
- `prob_V1_V2`: taxa de contaminação de V1 (doente) para V2 (saudável)

#### Como esses dados se comunicam?

## 3) Avaliação:
O que define o sucesso? 
Um modelo de Machine learning com 95% de precisão é bom o suficiente?


## 4) Features:

Quais partes de nossos dados vamos usar para nosso modelo? 
O dataset está preenchido com p_v1_v2
Temos também como fazer um Join de datasets para aumentar a feature


Como o que já sabemos pode influenciar isso?

## 5) Modelagem:
Qual modelo você deve escolher?
Uma regressão simples, máximo polinomial
Como você pode melhorá-lo? Como comparar com outros modelos?


## 6) Experimentação:
O que mais poderíamos tentar? 
Nosso modelo implantado faz o que esperávamos? 
Como as outras etapas mudam com base no que encontramos?
