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

Escolhemos a gravidade e o tempo como variáveis fundamentais e utilizando o teorema de Buckingham’s Pi podemos relacionar essas variáveis com as duas váriáveis restantes. Com isso obteremos 2 grupos sem dimensões que relacionam as váriaveis relevantes para o problema.

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

Resolvendo o sistema de equação das dimensões temos:

<img src="https://render.githubusercontent.com/render/math?math=a_1 = -1, b_1 = -1"> \
<img src="https://render.githubusercontent.com/render/math?math=a_2 = -1, b_2 = -2">

Então os dois grupos sem dimensão para o problema da queda livre são:

<img src="https://render.githubusercontent.com/render/math?math=\prod_1 = (\frac{v}{gt})"> \
<img src="https://render.githubusercontent.com/render/math?math=\prod_2 = (\frac{h}{gt^2})"> 

Dessa relação podemos deduzir que a altura do objeto em queda livre vai ser:

<img src="https://render.githubusercontent.com/render/math?math=h = k gt^2"> <br>

Onde k é uma constante que posse ser descoberta através de experimentação ou aplicando as equações de mecânica de newtom. Utilizando as equações de newtow descobrimos que altura da pedra <img src="https://render.githubusercontent.com/render/math?math=h"> em um tempo <img src="https://render.githubusercontent.com/render/math?math=t"> é descrito pela equação:

<img src="https://render.githubusercontent.com/render/math?math=h = \frac{1}{2}gt^2"> <br>

No nosso problema o objeto vai ser lançado de uma altura inicial <img src="https://render.githubusercontent.com/render/math?math=h_0"> e com uma velocidade inicial <img src="https://render.githubusercontent.com/render/math?math=v_0">. Com isso a nova altura do objeto a cada intevalo de tempo vai depender da posição que o objeto já se encontrava somado os deslocamento provocado pela velocidade que o objeto já se encontra somado ao deslocamento causada pela relação que encontramos observando as dimensões. Podemos representar esse modelo com a formula:

<img src="https://render.githubusercontent.com/render/math?math=h = h_0 %2B v_0t %2B \frac{1}{2}gt^2">

Com esse modelo podemos determinas altura exata do bojeto em queda livre no decorrer do tempo.

#### 2. Resolva numericamente as equações de movimento para um corpo em queda livre a partir de uma altura inicial e um valor de velocidade inicial, em uma dimensão. 


#### 3. Valide o modelo realizando um experimento análogo ao simulado e verifique a acurácia do modelo. (Sugestão: meça 10 ensaios e calcule a média e desvio padrão do experimento para comparar com o resultado simulado).

#### 4. Apresente os resultados  de forma gráfica, com as curvas da posição, velocidade e aceleração em função do tempo. Discuta os resultados e  apresente suas conclusões.

https://germanotm.github.io/free-fall/

# Instruções para rodar localmente

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
