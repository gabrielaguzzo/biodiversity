# Biodiversidade em Parques Nacionais Norte Americanos

# 1. Introdução
 
Esse projeto investiga espécies ameaçadas de extinção em 4 parques nacionais dos Estados Unidos da América. É parte integrante do curso de Data Science Foundations, do Codecademy. Os objetivos desse projeto são preparar os dados, realizar análises gráficas e, por fim, explicar os resultados do estudo com base em algumas questões levantadas.

As ferramentas utilizadas foram:

Python 3.0 (com as bibliotecas Pandas, Seaborn, Matplotlib, SciPy e Statsmodels)
Jupyter Notebook
Github

O dataset foi disponibilizado pelo Codecademy e provém do National Parks Service.
Nota: Os dados deste projeto são inspirados em dados reais, mas são principalmente fictícios.

# 2. Briefing

Esse projeto tem o objetivo de entender melhor as espécies observadas em cada parque, bem como seu estado de conservação.

Essas são as questões que esse projeto procura responder:

- Qual é a distribuição dos estados de conservação por categoria?
- Qual é a categoria mais ameaçada de extinção?
- Qual é o número de observações por parque?
- Dentro categoria mais protegida, qual espécie é mais observada em cada parque?
- Qual espécie é a mais observada em cada parque?

# 3. Resolução
## 3.1. Estrutura dos dados

O conjunto de dados "species.info.csv" contém dados sobre diferentes espécies e seu estado de conservação. Seus atributos são:

| Atributos |	Descrição |
| --------- | --------- |
| category | categoria da espécie |
| scientific_name | nome científico da espécie |
| common_names | nomes comuns das espécies |
| conservation_status | estado de conservação da espécie |

Os conjunto de dados "observations.csv" mantém registros de avistamentos de diferentes espécies em vários parques nacionais nos últimos 7 dias e traz informações sobre quatro parques nacionais: Great Smoky Mountains National Park, Yosemite National Park, Bryce National Park e Yellowstone National Park. Seus atributos são:

| Atributos |	Descrição |
| --------- | --------- |
| scientific_name | nome científico da espécie |
| park_name | nome do parque nacional |
| observations | número de observações da espécie |

Algumas alterações foram necessárias nos datasets, como a limpeza de linhas duplicadas, para evitar uma análise enviesada, e o preenchimento de valores nulos.


## 3.2. Visualização de dados e Insights

Para responder às questões do projeto e encontrar insights sobre os dados, gerei gráficos e tabelas que pudessem auxiliar no entendimento dos dados. A escolha do tipo de gráfico se deu em função dos tipos das variáveis envolvidas, e as tabelas foram utilizadas quando entendi que, por meio delas, o entendimento se tornaria mais objetivo.

_1. Distribuição dos estados de conservação por categoria_

![Alt text](image-1.png)

Pelo gráfico, observa-se que a categoria "Bird" é a que possui o maior número de espécies no estado de conservação "Species of Concern".

![Alt text](image-2.png)

A categoria "Mammal" representa o maior número de espécies em "Endangered".

![Alt text](image-4.png)

No estado de conservação "Threatened", a categoria "Fish" se destaca.

![Alt text](image-5.png)

E, por fim, em "In Recovery" a categoria "Bird" se destaca.

_2. Número de observações por parque_

![Alt text](image-6.png)

Por meio da tabela, vemos que o Yellowstone National Park registrou o maior número de observações nos últimos 7 dias, com 1.442.314 observações.

_3. Espécie mais observada em cada parque dentro da categoria mais protegida_

Primeiramente descobri que a categoria mais protegida é a categoria "Mammal", com 17,05% das espécies sob algum tipo de proteção, seguida da categoria "Bird" com 15,37%.

![Alt text](image-7.png)

A tabela acima apresenta o número total de observações da categoria "Mammal" em cada parque, considerando apenas as espécies sob algum tipo de proteção. O Yellowstone National Park apresentou o maior número de avistamentos dessa categoria. É importante observar que isso pode se dever ao fato desse parque também apresentar o maior número de observações de espécies no geral.

![Alt text](image-8.png)

A tabela acima apresenta qual espécie, dentro da categoria "Mammal" foi mais avistada em cada parque. Das 4 espécies, 3 são morcegos.

_4. Espécie mais observada em cada parque_

Para responder a essa pergunta, primeiro gerei um gráfico que apresentasse o número de espécies de cada categoria observada em cada parque. Assim, é possível já observar que em todos os 4 parques a categoria mais avistada foi a "Vascular Plant".

![Alt text](image-9.png)

A tabela abaixo apresenta, por fim, qual espécie foi mais avistada em cada parque.

![Alt text](image-10.png)

# 4. Conclusões

Este projeto foi capaz de fazer algumas visualizações de dados e também conseguiu responder as questões colocadas no início:

- Qual é a distribuição dos estados de conservação por categoria?

Em "Espécies de Preocupação" e "Recuperação", os pássaros se destacam.
Em "Ameaçadas", a categoria dos peixes se destaca.
Em "Ameaçados de Extinção", os mamíferos representam o maior número de espécies.

- Qual é a categoria mais ameaçada de extinção?

Mammal (Mamíferos).

- Qual é o número de observações por parque?

Yellowstone National Park: 1.442.314

Yosemite National Park: 862.836

Bryce National Park: 575.901

Great Smoky Mountains National Park: 431.378

- Dentro categoria mais protegida, qual espécie é mais observada em cada parque?

A categoria mais protegida é a categoria Mammal (mamíferos).

| Parque |	Espécie | Número de Observações |

| --------- | --------- |

| Great Smoky Mountains National Park | Myotis californicus | 97 |

| Yosemite National Park | Myotis yumanensis | 169 |

| Bryce National Park | Myotis austroriparius | 152 |

| Yellowstone National Park	| Taxidea taxus | 261 |

- Qual espécie é a mais observada em cada parque?

| Parque |	Espécie | Número de Observações |
| --------- | --------- |
| Great Smoky Mountains National Park | Sonchus asper ssp. asper	 | 147 |
| Yosemite National Park | Ivesia shockleyi var. shockleyi | 223 |
| Bryce National Park | Valerianella radiata | 176 |
| Yellowstone National Park	| Lycopodium tristachyum | 321 |

# 5. Pesquisas futuras

