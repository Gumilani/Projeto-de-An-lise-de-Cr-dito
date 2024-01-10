[![author](https://img.shields.io/badge/author-Gustavomilani-red.svg)](https://www.linkedin.com/in/gustavostafocker/) [![](https://img.shields.io/badge/python+-blue.svg)](https://www.python.org/downloads/)  ![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?s)

# Projeto de Análise de Crédito

<p align="center">
  <img alt="Tabela" width="60%" src="https://github.com/Gumilani/Projeto-de-Analise-de-Credito/blob/main/Imagem_Projeto.jpg">
</p>

## Objetivo do Projeto 

 Nesse projeto, exploraremos uma base de créditos, onde os dados estão em um formato CSV e contém informações de clientes de uma instituição financeira.  
  Temos como principal objetivo fazer uma análise da segunda coluna da base, onde ela é chamada de **default** e indica se o cliente é adimplente (`default = 0`), ou inadimplente (`default = 1`), ou seja, queremos entender melhor qual é o comportamento das pessoas que acabam não pagando suas dívidas e ficam inadimplentes no mercado.

**Abaixo pode acessar o link para conferir o projeto completo:**
 - [**Projeto no Google Colab**](https://colab.research.google.com/drive/1fm1h-chAMchZuB1Ex1x0xHLuTMaXrn6Z#scrollTo=VSsI7ZDGdgDC)

## Fonte dos Dados

*  Os dados foram obtidos a partir do curso Cientista de dados - EBAC

Para acesso a base -> [base](https://raw.githubusercontent.com/andre-marcos-perez/ebac-course-utils/develop/dataset/credito.csv)

## Tecnologias Utilizadas
<p align="left"> 
   <a href="https://www.python.org" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="python" width="40" height="40"/> </a> 
   <a href="https://seaborn.pydata.org/" target="_blank" rel="noreferrer"> <img src="https://seaborn.pydata.org/_images/logo-mark-lightbg.svg" alt="seaborn" width="40" height="40"/>
   <a href="https://matplotlib.org/" target="_blank" rel="noreferrer"> <img src="https://seeklogo.com/images/M/matplotlib-logo-7676870AC0-seeklogo.com.png" alt="matplotlib" width="40" height="40"/>
</p> 

## Destaques do Projeto
### Divisão do estudo:

Nessa análise de dados conseguimos separar as variáveis em dois tipos, em variáveis categóricas (são os que estão relacionados a categorias Exemplo: Sexo nele temos masculino ou feminino) e variáveis numéricas (são os que estão relacionados a números Exemplo: Uma pessoa pode ter 10,20,30... anos), com isso conseguimos futuramente fazer uma analise mais facil da base.

### Pontos de destaque:

#### Variáveis categóricas:

Conforme descrito na LGPD, existem algumas variáveis que não devemos utilizar para a análise de dados pois não são argumentos que influenciam nas decisões.

Baseado nisso, vamos começar nossas análises a partir da variável escolaridade e não da variável sexo.

* Escolaridade

<p align="center">
  <img alt="Tabela" width="100%" src="https://github.com/Gumilani/Projeto-de-Analise-de-Credito/blob/main/grafico_escolaridade.png">
</p>

Ao comparar os 3 gráficos apresentados, podemos verificar que a distribuição das frequências se mantêm praticamente no mesmo padrão.

Uma única diferença que vemos que é bem sutil porém existe, é que a probabilidade de uma pessoa com o doutorado ser inadimplente é maior do que a de uma pessoa com graduação, mas é uma diferença muito pequena e o comportamento das pessoas num geral se mantêm igual.

Desta forma a Escolaridade não é suficiente para explicar a questão da inadimplência.

* Salário Anual

<p align="center">
  <img alt="Tabela" width="100%" src="https://github.com/Gumilani/Projeto-de-Analise-de-Credito/blob/main/grafico_salario.png">
</p>

Mais uma vez percebemos um padrão de distribuição de frequeência nos 3 gráficos apresentados.

 Conseguimos observar que a maioria das pessoas recebe menos que 40k, vimos também que o maior número de pessoas inadimplentes são as pessoas que recebem menos que 40k.

Por fim temos mais uma categoria que não nos ajuda a explicar de forma clara a questão da inadimplência.

#### Variáveis numéricas:

* Quantidade de Transações nos Últimos 12 meses

<p align="center">
  <img alt="Tabela" width="100%" src="https://github.com/Gumilani/Projeto-de-Analise-de-Credito/blob/main/qtd_transacoes_12m.png">
</p>  

Acima conseguimos primeiramente perceber que a maioria dos clientes realizaram entre 20-40 e 60-80 transações nos últimos 12 meses.

 No caso de clientes adimplentes conseguimos perceber que a concentração de transações muda um pouco e fica entre 60-100, já para os clientes inadimplentes o pico que fica entre 20 - 60 transações.

Com essa análise conseguimos perceber que a variável de quantidade de transações no último ano nos ajuda a entender melhor sobre o comportamento das pessoas que se tornam inadimplentes.

* Valor das transações nos últimos 12 meses

<p align="center">
  <img alt="Tabela" width="100%" src="https://github.com/Gumilani/Projeto-de-Analise-de-Credito/blob/main/valor_transacoes_12m.png">
</p> 

Acima vemos que grande parte dos valores das transações ficam entre 1000 e 5000. Para os clientes que estão inadimplentes verificamos que o valor de transações nos últimos 12 meses gira em torno de 2500

Desta forma, é possível identificar um padrão de comportamento para os inadimplentes o que indica que podemos considerar mais uma variável que irá nos ajudar a explicar a questão da inadimplência dos clientes do banco.

* Quantidade de Transações nos Últimos 12 meses X Valor das transações nos últimos 12 meses

<p align="center">
  <img alt="Tabela" width="40%" src="https://github.com/Gumilani/Projeto-de-Analise-de-Credito/blob/main/qtd_valor.png">
</p> 

Conseguimos perceber com esse gráfico algumas coisas:

*   As pessoas que fazem um número alto de transações e um valor muito alto acabam não sendo inadimplentes.
*  Percebemos também que temos dois principais grupos das pessoas que acabam virando inadimplentes: um grupo com os valores de transação entre 1000-5000 e outro grupo com o valor de 7500-10000.
*  Observamos que a quantidade de transações é menos representativa que o valor das transações para determinar a inadimplência, porém é possivel perceber uma alta concentração de inadimplentes com poucas transações na faixa de valor entre 1000 e 5000.

## Conclusão

A ideia principal desse projeto foi compreender melhor o comportamento dos clientes de uma instituição financeira para prevenir a inadimplência, permitindo à instituição concentrar-se mais nesse público e evitar a inadimplência.

As análises foram divididas em duas etapas:

Primeiro foi feito uma análise das seguintes **Variáveis Categóricas**: **Escolaridade**, **Estado Civil**, **Salário Anual** e **Tipo do Cartão**.Através desta análise, pudemos perceber alguns padrões de comportamentos dos clientes como por exemplo:

- A Instituição financeira tem mais da metade dos clientes com graduação ou acima
- A maioria dos clientes ganham menos que 40k por mês
- A maioria possui o cartão blue.

Porém percebemos tambem que essas características são iguais ou muito parecidas entre as pessoas adimplentes e as inadimplentes e com isso não conseguimos chegar em uma afirmação do que leva ou não a pessoa ser inadimplente.

 Com isso chegamos em nossa segunda análise referente às **Variáveis Numéricas** que são elas: **Idade**, **Dependentes**, **Meses de Relacionamento**, **Quantidade de Produtos**, **Interações nos últimos 12 meses**, **Meses inativo nos últimos 12 meses**, **limite de crédito**, **Valor das transações nos últimos 12 meses** e **Quantidade de transações nos últimos 12 meses**. Através da observação dessas variáveis foi possível entender melhor o comportamento dos clientes que acabam cometendo a inadimplência.

 As variáveis (`Valor das transações nos últimos 12 meses`) e (`Quantidade de transações nos últimos 12 meses`) são as mais significativas  através das quais notamos que temos dois grandes grupos que tendem ser inadimplentes.

 - Pessoas que fazem transações entre 1000 e 2500 reais e tem um volume baixo de 10 a 60 transações
 - Pessoas que fazem transações entre 5000 e 10000 reais e tem um volume médio 50 a 80 transações.

Outro ponto importante observado é de que pessoas que fazem um volume alto de transações (acima de 80 no ano) e com valores muito altos (a cima 12500) não é um problema para essa instituição financeira pois esse grupo não tem nenhuma tendencia a se tornar inadimplente sendo portanto um grupo seguro para a institução financeira.

Desta forma, as variáveis numéricas, em especial (valor das transações nos últimos 12 meses) e (quantidade de transações nos últimos 12 meses) são as mais adequadas para que a instituição financeira possa realizar o trabalho preventivo de inadimplência.

## Contato

Estou sempre aberto para sugestões e melhorias do trabalho!

**Links para me acharem:**
* [LinkedIn](https://www.linkedin.com/in/gustavostafocker/)
* [GitHub](https://github.com/Gumilani)
* Email: gstafocker2000@gmail.com

  





