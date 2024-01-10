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

Primeramente comecei com a análise das variáveis categóricas e Conforme descrito na LGPD, existem algumas variáveis que não devemos utilizar para a análise de dados pois não são argumentos que influenciam nas decisões.

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



