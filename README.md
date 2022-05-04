# Taxa de transmissão de uma doença

### 1) Definição do problema: 

## Que problema estamos tentando resolver?  

Este case tem como objetivo avaliar os níveis de contaminação de um vírus no país X, gerando insights através de dados fornecidos pelo Gorverno.

![alt text](https://github.com/mcalmeida13/neoway-case/blob/main/img/2022-05-04_14-56.png?raw=true)




Sabe-se que a transmissão acontece de pessoa por pessoa, por isso elas devem estar conectadas de alguma maneira (familia, amizade ou trabalho). Foi fornecido um dataset com o nível de proximidade das pessoas e a frequência com que se encontram e a probabilidade da transmissão entre os indivíduos.

Já foi repassado também que a porbabilidade transmissão de um indivíduo A para B não é igual a de B para A, o que sugere que os atributos de cada indivíduo contribuem para a probabilidade de adoecer


![alt text](https://github.com/mcalmeida13/neoway-case/blob/main/img/2022-05-04_14-56.png?raw=true)

Além desse dataset, foi fornecido outro onde cada linha rep e cada pessoa possui um conjunto de atributos.
Este vírus afeta esta sociedade como descrito a seguir:
● a taxa de contaminação varia de pessoa para pessoa;
● a taxa de contaminação de uma pessoa A para B é diferente de B para A e depende
das características de ambas as pessoas (A e B);
● a contaminação só passa através de indivíduos conectados;
● não existe cura para essa doença;

Como pode ser formulado como um problema de Machine learning?
Quais features contribuem para a taxa de contaminação?
Usar algum algoritmo de regressão para prever o valor da probabilidade para a outra metade das pessoas
Podemos clusterizar os tipos de usuário e talvez usar como feature

### 2) Dados:
Se o Machine learning está obtendo insights de dados, quais dados temos? Como ele corresponde à definição do problema? 
Dataset com cada entrada sendo as características dos usuários
Dataset de interação
Nossos dados são estruturados ou não estruturados? 
Estruturados
Estático ou streaming?
Estáticos

### 3) Avaliação:
O que define o sucesso? 
Um modelo de Machine learning com 95% de precisão é bom o suficiente?


### 4) Features:

Quais partes de nossos dados vamos usar para nosso modelo? 
O dataset está preenchido com p_v1_v2
Temos também como fazer um Join de datasets para aumentar a feature


Como o que já sabemos pode influenciar isso?

### 5) Modelagem:
Qual modelo você deve escolher?
Uma regressão simples, máximo polinomial
Como você pode melhorá-lo? Como comparar com outros modelos?


### 6) Experimentação:
O que mais poderíamos tentar? 
Nosso modelo implantado faz o que esperávamos? 
Como as outras etapas mudam com base no que encontramos?
