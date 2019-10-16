## Realizando Pré-processamento de dados com Python

Utilizei quatro técnicas de pré-processamento de dados com algumas bibliotecas do Python

#### Removendo valores anômalos (outlier)

Dados antes do pré-processamento
![outliers](https://user-images.githubusercontent.com/15157510/66878954-a42a2580-ef92-11e9-93af-8d18dfb676cf.PNG)

Dados depois do pré-processamento
![outliers2](https://user-images.githubusercontent.com/15157510/66879022-df2c5900-ef92-11e9-94a8-77f2124d129c.PNG)

Podemos observar que após o processamento dos dados de exemplo, já não temos mais valores outliers (anômalos). A técnica aplicada remove esses dados discrepantes da nossa base de dados antes de uma análise mais profunda.

#### Discretização de dados

A discretização dos dados é utilizada para transformar variáveis númericas em categóricas. No exemplo abaixo, utilizei uma base de dados de hotéis. Transformei a variável floor(piso) em uma variável categórica.

No exemplo, os quartos foram classificados da seguinte forma:

* 1.0 - Muito pequeno
* 2.0 - Pequenho
* 2.5 - Médio 
* 3.0 - Grande
* 3.5 - Muito Grande

A imagem só exibe os 10 primeiros registros.

![discretizacao](https://user-images.githubusercontent.com/15157510/66879286-d5572580-ef93-11e9-914a-110322684f0b.PNG)

#### Normalização de dados (Norma L2)

Dados antes do pré-processamento
![normalizer1](https://user-images.githubusercontent.com/15157510/66879344-13544980-ef94-11e9-878b-fdf5e6e76fb2.PNG)

Dados depois do pré-processamento
![normalizer2](https://user-images.githubusercontent.com/15157510/66879384-2ff08180-ef94-11e9-8a9e-9e6badb2ed9c.PNG)

A normalização dos dados utiliza a norma L2. É bom dá uma pesquisada na net !!! Vale a pena...

#### Standartization de dados - MinMaxScaler

Dados antes do pré-processamento
![MinMaxScaler](https://user-images.githubusercontent.com/15157510/66879416-58787b80-ef94-11e9-94e6-2a8f07e2221c.PNG)

Dados depois do pré-processamento
![MinMaxScaler2](https://user-images.githubusercontent.com/15157510/66879448-7645e080-ef94-11e9-8d9d-1e248c3436e3.PNG)

Utilizando o "MinMaxScaler", podemos observar que todos os valores da nossa base de dados foram normalizados para ficar entre 0 e 1. Independente do valor original. Visualizando as imagens acima, podemos ver a diferença de distribuição dos dois gráficos.

#### Standartization de dados - StandardScaler

Dados antes do pré-processamento
![StandardScaler1](https://user-images.githubusercontent.com/15157510/66879531-d2a90000-ef94-11e9-964a-ba8493f099fa.PNG)

Dados depois do pré-processamento
![StandardScaler2](https://user-images.githubusercontent.com/15157510/66879533-d3da2d00-ef94-11e9-9e53-f22045565181.PNG)

O StandardScaler realiza uma normalização quase igual ao MinMaxScaler. A diferença está no intervalo de valores que é criado pelo StandardScaler. Ele amplia a margem dos respectivos registros da base de dados. Podemos observar que o intervalo dos valores estão entre -2 e 2.

