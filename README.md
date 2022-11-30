# Projeto Sobre Pesquisas Eleitorais do Brasil

### A pesquisa foi feita atráves de uma analise de sentimento usando python e a rede social Twitter.

Para ser realizado a extração dos dados do twitter foram utilizados as seguintes api "__python-twitter-vw__" e "__snscrape__" e para realizar a analise de sentimento foi utilizado a api "__textblob__" e para conseguir recolher informaçoes sobre as eleições foi utilizado a api do "basedosdados" que usa informações do poder360.

Para rodar os scripts é necessario ter o python instalado e o power bi para poder ver os graficos.

## Explicação sobre o script feito em python:

1. Primeiro bloco de comandos está realacionado á instalação das bibliotecas/api.
2. Segundo bloco de comandos está relacionado á importação dos comandos a serem utilizados
3. Terceiro bloco de comandos está relacionado á extração de dados do twitter, que funciona da seguinte maneira, primeiramente é definido a data de inicialização e a data final, logo em seguida o codigo vai entrar em loop, sendo assim definido pelo __for x in range(360):__ naqual 360 representa o número de dias, e o seguinte comando __if i>10:__ naqual o 10 representa a quantidade de dados a serem recolhidos em determinado dia, apos passar pelo IF o codigo ira incrementar uma data tanto inicial quanto final para poder rodar até a quantia de dias informado, sendo assim ira recolher 10 twites por dia durante 360 dias, logo em seguida todo o conteúdo extraido será colocado dentro de um dataframe.
4. Quarto bloco este terá a função de analisar o sentimento de cada frase extraido do twitter.
5. Quinto bloco e por fim este será realizado uma alteração na data e também será criado um novo dataframe com a junção da data e do sentimento e logo em seguida o dataframe será salvo como um arquivo .xlsx para poder ser utilizado no power bi.
6. Do 6º bloco até o 14° será realizado o mesmo procedimento para realizar a extração de dados dos seguintes candidatos: Lula, Ciro e Simone Tebet.
7. Neste bloco será feita a extração dos dados da eleição feitos pelo poder360, naqual a parte selecionada para a pesquisa será a do instituto Datafolha, nessa código o campo __billing_project_id=""__ requer o id de um projeto no google cloud para realizar o download.
8. Neste bloco acontecera o filtro a respeito do dataframe criado para coletar as informações especificas e será criado mais um arquivo .xlsx para ser utilizado no power bi.
## Link do Power BI:

<a href="https://app.powerbi.com/view?r=eyJrIjoiNzlmZDJjYTEtMWZmOS00M2ZlLTk5OWMtZTA4ZmIzOTNlMjAxIiwidCI6IjA0OTM1NTdlLTViYjQtNDVmOS1iNmRkLTdiMjI1OWYzYzMzOCJ9&pageName=ReportSection16c7b219a6672a80e4b2">Click aqui!</a>
