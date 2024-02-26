# <font color=MediumVioletRed><strong>Análise e Previsões de Dados do Câncer de Mama</strong></font>

<hr>

![detectando cancer](https://github.com/Adriano1976/Breast-Cancer-Analysis-and-Predictions/assets/17755195/bcdbed5e-9788-4814-8953-cd37ba35d201)


Olá visitantes,

Estou muito contente em compartilhar com vocês a "<strong>Análise e Previsões de Dados do Câncer de Mama</strong>". Este notebook é uma espécie de tutorial para os iniciantes em <strong>`Machine Learning`</strong>, e espero que seja útil para todos que desejam aprender mais sobre o assunto.

Sintam-se em casa e aproveitem a exploração dos dados e das previsões relacionadas ao câncer de mama!

###  <font color=MediumVioletRed><strong>Câncer de Mama</strong></font>

O câncer de mama é câncer que se forma nas células das mamas. <p> Surge nas células de revestimento (`epitélio`) dos ductos (`85%`) ou lóbulos (`15%`) no tecido glandular da mama. Inicialmente, o crescimento cancerígeno está confinado ao duto ou lóbulo ("in situ"), onde geralmente não causa sintomas e tem potencial mínimo de propagação (`metástase`). <br>
    
A maioria dos tipos de câncer de mama é fácil de diagnosticar por análise microscópica de uma amostra - ou biópsia - da área afetada da mama. Além disso, existem tipos de câncer de mama que requerem exames de laboratório especializados.

### <font color=MediumVioletRed><strong>Sobre o Conjunto de Dados e Suas Características</strong></font>

* Os conjuntos de dados de câncer de mama estão disponíveis no Repositório de <strong>`Machine Learning`</strong> da UCI mantido pela <strong>Universidade da Califórnia, Irvine</strong>.
* O conjunto de dados contém 569 amostras de células tumorais malignas e benignas.

* As duas primeiras colunas do conjunto de dados armazenam os números de ID exclusivos das amostras e o diagnóstico correspondente (M = `maligno`, b = `benigno`), respectivamente.
* As colunas 3-32 contêm 30 recursos de valor real que foram calculados a partir de imagens digitalizadas dos núcleos celulares, que podem ser usados para construir um modelo para prever se um tumor é benigno ou maligno.

    * 1 = maligno (`canceroso`) - ( M )
    * 0 = benigno (`não canceroso`) - ( B )     

#### <font color=MediumVioletRed><strong>Características Básicas do Tumor</strong></font>

- `diagnosis`: Esta característica indica se o tumor é benigno (B) ou maligno (M). É o alvo que os modelos de aprendizado de máquina tentam prever.
- `radius_mean`: Medida média do raio do tumor.
- `texture_mean`: Medida média da rugosidade da superfície do tumor.
- `perimeter_mean`: Medida média do contorno do tumor.
- `area_mean`: Medida média da área ocupada pelo tumor.
- `smoothness_mean`: Medida média da uniformidade da superfície do tumor.
- `compactness_mean`: Medida média da compacidade do tumor.
- `concavity_mean`: Medida média da concavidade do tumor.
- `concave points_mean`: Número médio de pontos côncavos no contorno do tumor.

#### <font color=MediumVioletRed><strong>Características nucleares do Tumor</strong></font>

- `texture_worst`: Medida da rugosidade da superfície do tumor, considerando a pior região.
- `perimeter_worst`: Medida do contorno do tumor, considerando a pior região.
- `area_worst`: Medida da área ocupada pelo tumor, considerando a pior região.
- `smoothness_worst`: Medida da uniformidade da superfície do tumor, considerando a pior região.
- `compactness_worst`: Medida da compacidade do tumor, considerando a pior região.
- `concavity_worst`: Medida da concavidade do tumor, considerando a pior região.
- `concave points_worst`: Número de pontos côncavos no contorno do tumor, considerando a pior região.
- `symmetry_worst`: Medida da simetria do tumor, considerando a pior região.
- `fractal_dimension_worst`: Medida da complexidade da forma do tumor, considerando a pior região.

#### Observações:

"`mean`" e "`worst`" indicam se a característica se refere a um valor médio calculado em todo o tumor ou ao valor máximo encontrado em qualquer região do tumor.
Essas características são medidas complexas derivadas de imagens de cortes histológicos de tumores de mama.
Interpretar cada característica individualmente pode ser difícil, mas elas são usadas em conjunto por modelos de aprendizado de máquina para prever o diagnóstico.

13 é o raio SE, o campo 23 é o pior raio.

    * Todos os valores dos recursos são recodificados com quatro dígitos significativos.

    * Valores de atributo ausentes: nenhum

> Distribuição de classe: 357 `Benigno`, 212 `Maligno`

<hr>
