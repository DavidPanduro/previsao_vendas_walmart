# previsao_vendas_walmart
Lojas Walmart fornece dados históricos de vendas para 45 das suas lojas localizadas em diferentes regiões. Cada loja contém uma série de departamentos, e temos a tarefa de prever as vendas em todo o departamento para cada loja.

Além disso, o Walmart realiza vários eventos promocionais de marcação ao longo do ano. Essas marcações precedem feriados proeminentes, os quatro maiores dos quais são o Super Bowl, Dia do Trabalho, Ação de Graças e Natal. As semanas incluindo esses feriados são ponderadas cinco vezes mais altas na avaliação do que as semanas sem feriados. Parte do desafio apresentado por esta competição é modelar os efeitos das marcações nestas semanas de férias na ausência de dados históricos completos/ideais.

lojas.csv

Este arquivo contém informações anonimizadas sobre as 45 lojas, indicando o tipo e o tamanho da loja.

treinamento.csv

Estes são os dados históricos de treinamento, que abrangem 2010-02-05 a 2012-11-01. Dentro deste arquivo, você encontrará os seguintes campos:

Loja - o número da loja
Departamento - o número do departamento
Data - a semana
Weekly_Sales - vendas para o departamento dado na loja dada
IsHoliday - se a semana é uma semana especial de feriado
teste.csv

Este arquivo é idêntico ao trem.csv, exceto que retivemos as vendas semanais. Você deve prever as vendas para cada trigêmeo de loja, departamento e data neste arquivo.

características.csv

Este arquivo contém dados adicionais relacionados à loja, departamento e atividade regional para as datas dadas. Contém os seguintes campos:

Loja - o número da loja
Data - a semana
Temperatura - temperatura média na região
Fuel_Price - custo do combustível na região
MarkDown1-5 - dados anonimizados relacionados a marcações promocionais que o Walmart está executando. Os dados do MarkDown só estão disponíveis após novembro de 2011, e não estão disponíveis para todas as lojas o tempo todo. Qualquer valor perdido é marcado com um NA.
IPC - o índice de preços ao consumidor
Desemprego - a taxa de desemprego
IsHoliday - se a semana é uma semana especial de feriado

Por conveniência, os quatro feriados caem nas semanas seguintes no conjunto de dados (nem todos os feriados estão nos dados):
Super Bowl: 12-Feb-10, 11-Feb-11, 10-Feb-12, 8-Feb-13
Dia do Trabalho: 10-Set-10, 9-Set-11, 7-Set-12, 6-Set-13
Ação de Graças: 26-Nov-10, 25-Nov-11, 23-Nov-12, 29-Nov-13
Natal: 31-Dez-10, 30-Dez-11, 28-Dez-12, 27-Dez-13
