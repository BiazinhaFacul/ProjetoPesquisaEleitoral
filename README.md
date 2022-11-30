## Projeto: Pesquisas Eleitorais no Brasil

### A pesquisa foi feita atráves de uma análise de sentimento usando Python e a rede social Twitter.

Para executar os scripts é necessario ter o Python instalado e o Power BI para poder ver os gráficos.

## Explicação do script feito em Python:

1. Primeiro bloco de comandos está realacionado a instalação das bibliotecas/api.
2. Segundo bloco de comandos está relacionado a importação dos comandos que serão utilizados
3. Terceiro bloco de comandos está relacionado a extração de dados do twitter, que funciona da seguinte forma, primeiro é definido a data de inicialização e a data final, logo em seguida o código vai entrar em loop, sendo assim definido pelo __for x in range(360):__ na qual 360 representa o número de dias, e o seguinte comando __if i>10:__ na qual o 10 representa a quantidade de dados a serem recolhidos em determinado dia, após passar pelo IF o código irá incrementar uma data tanto inicial quanto final para poder executar até a quantia de dias informado, sendo assim, irá recolher 10 twittes por dia durante 360 dias, logo em seguida todo o conteúdo extraído será colocado dentro de um dataframe.
4. Quarto bloco, este terá a função de analisar o sentimento de cada frase extraída do twitter.
5. Quinto bloco, este será realizado uma alteração na data e também será criado um novo dataframe com a junção da data e do sentimento, será dividido em positivo e negativo e logo em seguida será salvo em dois arquivos .xlsx separados para poderem ser utilizados no Power BI.
6. Do 6º bloco até o 14°, será realizado o mesmo procedimento para realizar a extração de dados dos seguintes candidatos: Bolsonaro, Ciro, Lula e Simone Tebet.
7. No bloco 15º será feita a extração dos dados da eleição feitos pelo jornal Poder360, na qual a parte selecionada para a pesquisa será a do instituto Data Folha. Nesse código o campo __billing_project_id=""__ requer o Id de um projeto no Google Cloud para realizar o download.
8. No bloco 16º acontecerá o filtro a respeito do dataframe criado para coletar as informações específicas, e será criado mais um arquivo .xlsx para ser utilizado no Power BI.
## Link do Power BI:

<a href="https://app.powerbi.com/view?r=eyJrIjoiZjU1YTI3ZGMtN2Y3Ny00Mzc3LWE2ZjAtMTQ4YjhjMzUyZjcyIiwidCI6IjA0OTM1NTdlLTViYjQtNDVmOS1iNmRkLTdiMjI1OWYzYzMzOCJ9&pageName=ReportSection761bb02f22247301ec5a">Link para visualização do Power BI.</a>

