# Fundamentos_power_BI

*grupo Voitto*

O que podemos fazer com o power BI:

  - construir relatórios;
  - vizualizar os dados;
  - analisar os dados, criando insights;
  - compartilhar as suas informações;
  
  <br>
Business Intelligence é um termo que se refere ao processo de colata, oraganização, análise, compartilhamneto e monitoramento de informações, auxiliando a gestão de negócios. Pensando no foco e resultado. <br>
 
<h3>Conectando banco de dados ao Power BI</h3>

O Power BI suporta uma grande variedade de fontes de dados. Podendo conctar-se com varios tipos de arquivos, como Excel, bancos de dados SQL e nuvem Azure, e em plataformas da Web como objetos do Facebook, google analytics e salesforce. E até mesmo de ODBC, que são bancos de dados mais complexos.<br>

<h3> Importando dados para o Pwer BI</h3>

Para importar os dados é simples:

* 1º: Obter dados > arquivo > escolha o arquivo e conecte > okay;
* 2º : clique no checbox do arquivo > carregar;

*Quando for exportar uma base de dados csv, prestar atenção qual é o tipo que está sendo identificado, para ele não vir com informaçãoes "bagunçadas" e com dificil compreensão. Então caso isso ocorra, em origem do arquivo, antes de carregar, clique em 65001:Unicode(UFT-8)*. <br>

* Para puxar dados de uma pagina Web, é simples: obter dados > web > você copia o link do site que tenhas as informações que você quer analisar > você escolhe qual é a tabela com as informações que você quer> de um chackbox na tabela > carrega;

Relacionamento é a existencia de uma informação em comun entrer duas ou mais tabelas, e as relações entre essas tabelas são necessárias para calcular os resultados com precisõa e exibir as informações corretas em seus relatórios. 

*PROCV e PROH, no excel?*

Elas atuam de forma similar "procuram" uma determinada informação de uma tabela em outra para assim "trazer" um novo campo. 

Para fazer um relacionamento de tabelas, você carrega a primeira bade de dados que vai ultilizar, em vez de carregar você clica em transformar e assim você analisa as tabelas. Exemplo: Se há vairas colunas nulas (null), você seleciona todas através, clicando a primeira coluna então aperte o Shift e depois a ultima e assim, você seleciona todas e depois você clica em excluir colunas. Alterar as colunas que fazem referencia a valores monetários, botão direito no cabeçalho da tabela, alterar valor, numero decimal fixo  ele muda para tipo monetario. Mudar data para tipo data. Depois de "arrumados". Você clica em novas fontes. E você seleciona o tipo do arquivo que você vai puxar, caso seja necessarios faça as alterações. E assim que terminar você clica na barra de ferramentas, fechar e aplicar. <br>

*Preste atenção ao fazer o relacionamento, so deixe habilitado automaticamente se você fez uma pré analise nos dados e conhece as bases de dados, caso não tenhas esses requisitos, o melhor é o amnual para que não haja o problema de fazer uma analise na qual não faça sentido e não esteja certa.*

Caso ele esteja automatico, apague: passe o mouse na ordem de coneção, botão direito, excluir.<br>
Para fazer um relacionamento é simples, clique nas colunas que são iguais, primeiro em uma e depois você arrasta até o outro. Ou você tem aopção de ir na pagina inicial, gerenciar relações, selecione as colunas para fazer a relacionamento entre eles. 

<h3>Dax</h3>

Dax (data analystic Expressions), é o nome da linguagem formula usada pelo Power BI. <br>

Ele auxilia na extração e na ciração de informações dos seus dados através de uma coleção de funções, operadores e constantes que aparecem em uma fórmula ou expressão. <br>

Possui similaridade com o VBA(visual basic for application), a linguadem utilizada pela microsoft em seus demais produtos como o excel. <br> 

* Sintaxa:

  *= [VolumeDeVendas] - [CustoTotal]*<br>
  - inicia com o operador de igual, sempre que formos calcular, pois, é quando a calculadora retornará o resultado ou valor.
  - primeira coluna referenciada;
  - o sinal, o que a conta ira fazer;
  - segunda coluna referenciada;
 <br>
 
 **A linguagem Dax ultiliza operadores para criar expressões que comparam valores, executar calculos e trabalhar com cadeias de carateres.** <br>
* aritmético:<br>
   - (+) adição,
   - (-) subtração,
   - (*) multiplicação, 
   - (/) divisão), 
   - (^) potência;
* comparação:<br>
   - (=) igual,
   - (==) estrito igual a,
   - (>) maior que,
   - (<) menor que,
   - (>=) maior ou igual a,
   - (<=) menor ou igual a,
   - (<>) diferente de;
* texo:<br>
  - ( & ) conecta ou cocatenar dois valores para produzir um valor  de texto continuo;
* lógicos:
  - ( && ) cria uma condição *AND* entre duas expressões que têm um resultado booleano. Se ambas as expressões também retornarem TRUE, a combinação das expressões também serão TRUE, caso ao contrario a combinação retornará False,
  - ( || ) (cria uma condição *OR* entre duas expressões lógicas. Se uma das expressões retornar TRUE, o resultado será TRUE, quando as duas expressões são FALSE retornará FALSE,
  - ( IN ) cria uma condição *OR* lógica ente cada linha sendo comparada a uma tabela. Observação: a sintaxe do contrutor de tabelas usa chaves. Ex de cores;
  
Para criar uma nova coluna, iremos na parte de tabelas no Power BI, e na barra de ferramentas iremos clicar em criar uma nova coluna, e antes do *=* você escreve qual é o nome que você quer deixar na sua coluna, e logo em seguida você começa selecionar, e calcular as informações que você deseja para essa nova coluna. <br>

<h3>Dashboard</h3>

O Power BI possui uma grande variedade de visualizações que você pode escolher para exibir os seus dados e resultados. O Conjunto dessas vizualições de forma organizada e com um objetivo forma um Dashboard!

Dashboard são graficos organizados de uma maneira que você possa contar historias. <br>

Pontos relevantes:
* é uma página unica, geralmente chamada de tela, que conta uma historia por meio de visualizações,
* por ser limitado a uma unica página, um dashboard bem projetados contém apenas os elementos mais importantes da história. 
* os leitores podem exibir relatorios relacionados para obter detalhes;

*Gráficos*

São representções visuais utilizadas para exibir informações u valores numéricos que servem para demonstrar padrões tendencias ou camparar informações qualitativas e quantitativas em um determinado espaço de tempo.

**Como escolher o melhor gráfico**

faça três perguntas:<br>
  - O que você pretende mostrar com o seu gráfico?
  - Quantas variaveis e categorias seu grafico irá mostrar?
  - Quem é o publico que vai ler os seus gráficos?
<br>
* Graficos para comparar valores: <br>
  - caso seja preciso confrontar valores ao longo do tempo ou entre varias categorias, prefira os gráficos de Barras e Colunas;
  
* Graficos para mostrar representatividade:<br>
  - pizza, rosca e treemap;
  
* Gráfico para analisar a tendencias de dados:<br>
  - linhas e de área, mostra como se comporta;
* Gráfico acompanhar ganhos e perdas:<br>
  - grafico cascata;
  
* Gráfico acompanhamento de meta:<br>
  - KPI ou grafico de velocimetro;
* Gráfico compreender a distribuição de dados:<br>
  - grafico de dispersão;
* Gráfico para entender a relação entre conjunto de dados:<br>
  - combinado de barras e colunas;
 




