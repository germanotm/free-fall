# Princípios de Modelagem Matemática - Queda Livre
Aluno: Germano Teixeira de Miranda
Professor: Albens Atman

O objetivo do trabalho é assimilar o conceito de modelagem matemática e computacional a partir de um problema do mundo real.

#### 1. Equacione o problema da queda livre em uma dimensão construindo o modelo matemático.

As grandezes relevantes para o problema da queda livre são <img src="https://render.githubusercontent.com/render/math?math=V"> - Velocidade, <img src="https://render.githubusercontent.com/render/math?math=h"> - Altura, <img src="https://render.githubusercontent.com/render/math?math=t"> - Tempo e <img src="https://render.githubusercontent.com/render/math?math=g"> - Gravidade. 

Suas respectivas dimensões são:

<img src="https://render.githubusercontent.com/render/math?math=[V] = \frac L T "> \
<img src="https://render.githubusercontent.com/render/math?math=[h] = L ">
<img src="https://render.githubusercontent.com/render/math?math=[t] = T ">
<img src="https://render.githubusercontent.com/render/math?math=[g] = \frac L {T^2} ">

Nesse problema temos 4 variáveis <img src="https://render.githubusercontent.com/render/math?math=(V,h,t,g)"> e duas grandezas fundamentais <img src="https://render.githubusercontent.com/render/math?math=(T,L)">.

Escolhemos a gravidade e o tempo como variáveis fundamentais e utilizando o teorema de Buckingham’s Pi podemos relacionar essas variáveis com as duas variáveis restantes. Com isso obteremos 2 grupos sem dimensões que relacionam as variáveis relevantes para o problema.

<img src="https://render.githubusercontent.com/render/math?math=\prod_1 = V^{a_1} t^{b_1} g"> \
<img src="https://render.githubusercontent.com/render/math?math=\prod_2 = V^{a_2} t^{b_2} h">

Substituindo as respectivas dimensões temos:

<img src="https://render.githubusercontent.com/render/math?math=\prod_1 = (LT^{-2})^{a_1} T^{b_1} LT^{-1}"> \
<img src="https://render.githubusercontent.com/render/math?math=\prod_2 = (LT^{-2})^{a_2} T^{b_2} L"> 

De <img src="https://render.githubusercontent.com/render/math?math=\prod_1"> temos:

<img src="https://render.githubusercontent.com/render/math?math=L: a_1 %2B 1 = 0 "> \
<img src="https://render.githubusercontent.com/render/math?math=T: -2a_1 %2B b_1 - 1 = 0 ">

De <img src="https://render.githubusercontent.com/render/math?math=\prod_2"> temos:

<img src="https://render.githubusercontent.com/render/math?math=L: a_2 %2B 1 = 0 "> \
<img src="https://render.githubusercontent.com/render/math?math=T: -2a_2 %2B b_2 = 0 ">

Resolvendo o sistema de equações temos:

<img src="https://render.githubusercontent.com/render/math?math=a_1 = -1, b_1 = -1"> \
<img src="https://render.githubusercontent.com/render/math?math=a_2 = -1, b_2 = -2">

Então os dois grupos sem dimensão para o problema da queda livre são:

<img src="https://render.githubusercontent.com/render/math?math=\prod_1 = (\frac{v}{gt})"> \
<img src="https://render.githubusercontent.com/render/math?math=\prod_2 = (\frac{h}{gt^2})"> 

Dessa relação podemos deduzir que a altura do objeto em queda livre vai ser:

<img src="https://render.githubusercontent.com/render/math?math=h = k gt^2"> <br>

Onde k é uma constante que posse ser descoberta através de experimentação ou aplicando as equações de mecânica de newton. Utilizando as equações de newton descobrimos que altura da pedra <img src="https://render.githubusercontent.com/render/math?math=h"> em um tempo <img src="https://render.githubusercontent.com/render/math?math=t"> é descrito pela equação:

<img src="https://render.githubusercontent.com/render/math?math=h = \frac{1}{2}gt^2"> <br>

No nosso problema o objeto é lançado de uma altura inicial <img src="https://render.githubusercontent.com/render/math?math=h_0"> e com uma velocidade inicial <img src="https://render.githubusercontent.com/render/math?math=v_0">. Com isso a nova altura do objeto a cada intervalo de tempo vai depender da posição que o objeto já se encontrava somado ao deslocamento provocado pela velocidade que o objeto já se encontra somado ao deslocamento causada pela aceleração que encontramos observando as dimensões. Podemos representar esse modelo com a formula:

<img src="https://render.githubusercontent.com/render/math?math=h = h_0 %2B v_0t %2B \frac{1}{2}gt^2">

Com esse modelo podemos determinar a altura exata do objeto em queda livre no decorrer do tempo.

#### 2. Resolva numericamente as equações de movimento para um corpo em queda livre a partir de uma altura inicial e um valor de velocidade inicial, em uma dimensão. 

Soltando um objeto de uma altura inicial <img src="https://render.githubusercontent.com/render/math?math=h_0 = 100m"> com uma velocidade inicial <img src="https://render.githubusercontent.com/render/math?math=v_0 = -2m/s"> vamos aplicar o modelo para um intervalo de tempo igual a 1 segundo:

<img src="https://render.githubusercontent.com/render/math?math=h_1 = h_0 %2B v_0t %2B \frac{1}{2}gt^2"> \
<img src="https://render.githubusercontent.com/render/math?math=h_1 = 100 - 2*1 %2B \frac{1}{2}*(-9.8)*1">
<img src="https://render.githubusercontent.com/render/math?math=h_1 = 93.1 m">

Podemos verificar a nova velocidade no momento avaliando a distância percorrida pelo objeto no ultimo intervalo de tempo através da formula.

<img src="https://render.githubusercontent.com/render/math?math=v_1 = \frac{h_1 - h_0}{t} = \frac{93.1 - 100}{1} = -6.9 m/s">

Repetimos o passo para descobrir a altura da pedra no tempo <img src="https://render.githubusercontent.com/render/math?math=t = 2">:

<img src="https://render.githubusercontent.com/render/math?math=h_2 = h_1 %2B v_1t %2B \frac{1}{2}gt^2"> \
<img src="https://render.githubusercontent.com/render/math?math=h_2 = 93.1 - 6.9*1 %2B \frac{1}{2}*(-9.8)*1">
<img src="https://render.githubusercontent.com/render/math?math=h_2 = 78.6 m">

<img src="https://render.githubusercontent.com/render/math?math=v_2 = \frac{h_2 - h_1}{t} = \frac{78.6 - 93.1}{1} = -14.5 m/s">

Esse processo vai continuar até que o objeto se encontre com o solo.


#### 3. Valide o modelo realizando um experimento análogo ao simulado e verifique a acurácia do modelo. (Sugestão: meça 10 ensaios e calcule a média e desvio padrão do experimento para comparar com o resultado simulado).

Utilizando as leis de movimento de newton podemos ver que a equação de descreve o deslocamento de um corpo em aceleração é:

<img src="https://render.githubusercontent.com/render/math?math=S = \frac{1}{2}at^2"> 

Também temos na mecânica clássica que o deslocamento de um corpo é proporcional à sua velocidade e do tempo. 
<img src="https://render.githubusercontent.com/render/math?math=S = vt">

O nosso modelo retrata a mesma situação com um corpo acelerando na vertical com a aceleração da gravidade <img src="https://render.githubusercontent.com/render/math?math=g">.

#### 4. Apresente os resultados  de forma gráfica, com as curvas da posição, velocidade e aceleração em função do tempo. Discuta os resultados e  apresente suas conclusões.

A simulação do modelo está disponível em [Simulação do modelo](https://germanotm.github.io/free-fall/). Preencha os valores de altura inicial e velocidade inicial e clique em simular para observar os resultados.

A imagem abaixo mostra um exemplo de resultado:

# Instruções para rodar localmente

Criei uma aplicação vue e implementei em js a simulação do modelo proposto para queda livre. O principal objetivo de ter escolhido js como linguagem foi para utilizar WebGL para visualização da simulação. O WebGL é desnecessário para visualizar essa simulação pois ela pode ser facilmente representada em um gráfico 2D, mas optei por utilizar mesmo assim porque acredito que uma ferramenta gráfica mais poderosa vai ser muito útil para simulações futuras de modelos mais complexos. 

## Project setup
```
yarn install
```

### Compiles and hot-reloads for development
```
yarn serve
```

### Compiles and minifies for production
```
yarn build
```

### Lints and fixes files
```
yarn lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).
