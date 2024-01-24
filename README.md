## Projeto Final Curso de Análise de Dados em Python - Zênite Serena - Desmatamento e Agropecuária no Brasil

### Contextualização e Resumo da Análise

Projeto final apresentado ao final do bootcamp "Python: Fundamentos e Análise de Dados" da [{reprograma}](https://reprograma.com.br/curso-python/), realizado no segundo semestre de 2023. O projeto foi realizado ao longo das semanas 17 e 18 do curso.

[Repositório no GitHub](https://github.com/zenite-serena/Desmatamento-e-Agropecuaria-no-Brasil)

[Dashboard no Tableau](https://public.tableau.com/views/ProjetoFinal-Reprograma-on26-ZniteSerena/DesmatamentoCO2eProduodealimentos)

A crise climática representa o maior desafio já enfrentado pela humanidade. Trata-se de um problema multifacetado, mas com alguns determinantes centrais: o aquecimento global causado pela emissão de gases do efeito estufa (sobretudo o dióxido de carbono, CO2), o desmatamento de florestas nativas, o aumento do nível do mar devido ao derretimento das calotas polares e a subsequente queda em biodiversidade que estes problemas acarretam.

O desmatamento é a segunda maior fonte antropogênica de gases do efeito estufa (Pendrill et al., 2019), então este foi o foco da nossa análise: a relação entre *desmatamento e produção agropecuária no Brasil*.

A análise envolveu o tratamento de dados relacionados a desmatamento, produção de alimentos e atividades econômicas no Brasil, com o objetivo de gerar visualizações que dessem dimensões para o problema a ser enfrentado.

<img aria-label="Relação entre Desmatamento, CO2 e Produção de Alimentos" src="material\estrutura-projeto\dashboard\Desmatamento, CO2 e Produção de alimentos.png" width='70%'/>

Para isso, partimos de dados disponíveis em revistas científicas relacionando o desmatamento à produção de alimentos, que apontaram o Brasil como grande desmatador a nível mundial. Os dados também apontaram que a produção agropecuária é uma grande responsável pelo desmatamento e produção de CO2. A produção de colheitas comerciais também tem um papel importante no problema. 

<img aria-label="Gráfico de principais produtos de exportação" src="material/estrutura-projeto/dashboard/Exportação%20Agropecuária.png" width='70%'/>

Posteriormente, utilizamos dados do Instituto Brasileiro de Geografia e Estatística (IBGE) para olhar para o papel econômico da produção agropecuária. Atualmente, a produção de soja - uma das principais colheitas comerciais - é em sua maioria voltada à exportação. Produtos relacionados a culturas não perenes e processamento de carne também têm relevância neste contexto.

<img aria-label="Produção agropecuária no Brasil" src="material\estrutura-projeto\dashboard\Produção agropecuária.png" width='70%'/>

Os dados do IBGE também apontam para o crescimento na produção de cana-de-açúcar, soja e carne bovina.

### Tratamento de dados

Ao todo, trabalhamos com 9 bases de dados e geramos 8 bases após o tratamento.

Os bancos de dados retirados do site ourworldindata.org necessitaram de pouco tratamento, dado que estavam disponibilizados já tratados, assim como acompanhados de visualizações em gráficos, de modo que o trabalho da primeira parte do exercício consistiu basicamente no ranqueamento de valores, seleção de linhas, remoção de colunas, arredondamento de valores e tradução de colunas para o português. Após esse leve tratamento, plotamos gráficos que se assemelham àqueles disponíveis no site, então frisamos que o exercício consiste mais na prática no uso de funções da biblioteca matplotlib do que propriamente na criação de gráficos inéditos. 

Para a segunda parte da análise, feita a partir de dados do IBGE, foi necessário mais tratamento de dados, visto que os bancos de dados não estavam tão apropriados para o que pretendíamos fazer. Foram necessários o tratamento de dados nulos ou NaN, a transposição de linhas e colunas, a remoção de colunas e linhas, a renomeação de colunas, a modificação do tipo de dados, arredondamento de valores, remoção de dados string e slicing para criação de subsets.

Foram utilizadas as bibliotecas Pandas e Matplotlib.

### Conclusão

As visualizações explicitam a dimensão do problema a ser enfrentado quando falamos de mudança climática. Se um dos determinantes centrais desta mudança é a emissão de CO2 que resulta no aquecimento global, e sendo o desmatamento a segunda maior fonte antropogênica de gases do efeito estufa, é inegável que a economia do nosso país contribui para o problema, com seu foco na produção agropecuária para exportação.

É um desafio multifacetado e com inúmeros desdobramentos, mas um possível primeiro passo para o enfrentamento é o reconhecimento das suas principais causas, para que seja possível efetuar mudanças significativas no rumo que se tem tomado até aqui.

### Visualizações

[Dashboard no Tableau](https://public.tableau.com/views/ProjetoFinal-Reprograma-on26-ZniteSerena/DesmatamentoCO2eProduodealimentos)

Na pasta 'dashboard' é possível encontrar o arquivo do dashboard em extensão .twbx assim como imagens dos dashboards em .png.

## Referências: 

### Visualização de dados:

[Python Graph Gallery](https://python-graph-gallery.com/)

[Documentação MatPlotLib](https://matplotlib.org/)

[Data to Viz Project](https://www.data-to-viz.com/)

### Desmatamento de florestas tropicais:

["Deforestation and Forest Loss"](https://ourworldindata.org/deforestation)

["Cutting down forests: what are the drivers of deforestation?"](https://ourworldindata.org/what-are-drivers-deforestation)

["Is our appetite for soy driving deforestation in the Amazon?"](https://ourworldindata.org/soy)

### Produção agropecuária no Brasil
[Sistema IBGE de Recuperação Automática - SIDRA - Acervo](https://sidra.ibge.gov.br/Acervo)

[Sistema IBGE de Recuperação Automática - SIDRA - Tabelas específicas](https://sidra.ibge.gov.br/tabela/6588)


[Ministério da indústria, comércio exterior e serviços (Comex Stat - Exportação e Importação Geral)](http://comexstat.mdic.gov.br/pt/geral/86263)

["Complexo da Soja: Análise dos dados nacionais e internacionais" (2019)](https://thetricontinental.org/pt-pt/brasil/complexo-da-soja-analise-dos-dados-nacionais-e-internacionais/)
