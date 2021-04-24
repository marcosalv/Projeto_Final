<img src="https://bit.ly/2VnXWr2" alt="Ironhack Logo" width="100"/>

# O impacto da política de Auxílio Emergencial no enfrentamento da Pandemia
*Marcos Pereira Alves*

*São Paulo, 24 de Abril de 2021*

## Content
- [Descrição do projeto](#project-description)
- [Hipóteses e questionamentos](#hypotheses-/-questions)
- [Dataset](#dataset)
- [Cleaning](#cleaning)
- [Analysis](#analysis)
- [Conclusão](#conclusion)
- [Future Work](#future-work)
- [Workflow](#workflow)
- [Links](#links)

<a name="project-description"></a>

## Descrição do Projeto
Este projeto visa verificar se existiu correlação entre as políticas de distribuição de renda, específicamente auxílio emnergencial, e a número de casos de covid-19 no Brasil.

<a name="hypotheses-/-questions"></a>

## Hypotheses / Questions
* Existe correlação entre o ínicio da distrubição de Auxílio Emergencial e o número de casos de Covid-19 no Brasil? 
* Estados que receberam maior renda per capta de auxílio emergencial obtiveram menor número de casos de Covid-19? 
* O auxílio emergencial impactou algum outro campo da economia?  
Frame your hypothesis with statistical/data language (i.e. define Null and Alternative Hypothesis). You can use formulas if you want but that is not required.

<a name="dataset"></a>

## Dataset
* Dados públicos de auxílio emergencial extraídos do link abaixo:
* [Auxílio Emergencial](http://portaltransparencia.gov.br/download-de-dados/auxilio-emergencial)
* Dados públicos de casos de Covid-19 no Brasil extraídos de:
* [Dados Covid](https://covid.saude.gov.br/)
* Dados de consumo e confiança do consumidor extraídos de:
* [Indíce de confiança do consumidor](https://www.fecomercio.com.br/pesquisas/indice/icc)

<a name="cleaning"></a>

## Cleaning
Para o dataset de auxílio emergencial foi necessário maior complexidade computacional pois os dados são mensais com bases completas de número de pessoas, as variações de peso são de 6gb até 15gb. Dentro do processo de Cleaning, foram realizados alguns drops de colunas que não traziam dados de localização. Os dados de bloqueio de benefício e não distribuição por alguma pendência específica também foram retírados para não inviezar a análise.
O dataset de Covid-19 possuia estrutura menos complexa, foram feitas limpezas em colunas de localização e código de municípios.
Para o dataset de confiança do consumidor não foi o processo de cleaning, toda a base foi importada diretamente para o Tableau.

<a name="analysis"></a>

## Analysis
* Foi realizada uma comparação entre o número de novos casos a partir do início da distribuição de auxílio emergencial no país, para isso foi necessário correlacionar os dados  no Tableau.
* Após isso, foram construídos gráficos de geolocalização para mostrar as realidades de densidade populacional, número de casos no país e renda média per capta recebida por pessoas com direito ao auxílio emergencial.
* Para explorar dos dados, foram criadas alguns campos cálculados com descrição no link disponibilizado abaixo.
* [Análise Tableau](https://public.tableau.com/profile/marcosalv#!/vizhome/ProjetoFinal_2_16190508203340/Histria1?publish=yes) 



<a name="conclusion"></a>

## Conclusão
* Pela interpretação dos dados, foi possível identificar que somente com a implementação de auxílio emergencial não existe impacto direto na redução de número de casos.
* O auxílio emergencial foi distribuido durante 9 meses no ano de 2020  como uma das medidas de retenção para o avanço dos casos em todo o Brasil, mas o principal motivo do mesmo era garantir renda mínima para a população mais necessitada.
* O auxílio emergencial sozinho pode não impactar diretamente no número de casos de Covid-19 no país, no entanto, tem relacionamento direto com a confiança do consumidor, a partir da sua implementação surge a estabilidade do indicador frente ao mercado contribuindo para a aceleração da economia que é um dos principais efeitos colaterais da pandemia no mundo.

<a name="future-work"></a>

## Future Work
Analisar os dados de 2021 e entender quais os outros fatores além da suspensão incial do auxílio emergencial impactou no aumento da taxa de contaminação de covid-19 no país.

<a name="workflow"></a>

## Workflow
* Download dos datasets.
* Processo de cleaning e ajuste de estruturas no Jupter Noteebok com Python.
* Exportar datasets e consolidados dados no Tableau.
* Comparação com dados governamentais totalitários e análises a nível granular disponíveis nos gráficos gerais da análise.

<a name="organization"></a>

<a name="links"></a>

## Links

[Repository](https://github.com/marcosalv/Projeto_Final)  
[Slides](https://public.tableau.com/profile/marcosalv#!/vizhome/ProjetoFinal_2_16190508203340/Histria1?publish=yes)  
 
