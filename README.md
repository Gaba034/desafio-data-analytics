# Adição de pacote essêncial para o funcionamento do código.

Para a funcionalidade total desse código, adicione o arquivo *"bcim_2016_21_11_2018.gpkg"* que se encontra presente no repositório

> https://github.com/Gaba034/desafio_manchester

De maneira explicativa:

* Entre no repositório https://github.com/Gaba034/desafio_manchester
* Faça o download do arquivo *"bcim_2016_21_11_2018.gpkg"*
* Entre no repositório https://github.com/Gaba034/desafio-data-analytics
* Faça um git clone ou baixe o repositório
* Adicione o arquivo na raiz desse repositório que acabou de clonar ou baixar.

Com essa adição um dos gráfico poderá ser exibido de forma clara e explicativa.

# Caso não adicione:

Um dos gráficos depende desse pacote de geo dados, sem essa adição não será possivel a geração dele.

---

# Relatório para a empresa XYZ.

Data: 10 de junho, 2023

Para: Empresa XYZ

De: Gabriel Kalinoski

Assunto: Relatório de Análise de Dados


Espero que este relatório encontre você bem. Como Analista de Dados, tive o prazer de realizar uma análise completa dos dados da empresa nos últimos meses. Com base nas informações coletadas, apresento abaixo os principais insights e recomendações para ajudar na tomada de decisões informadas.

# Resumo Executivo:
A seguir, apresentarei um resumo com as informações mais relevantes, seguido por uma análise mais detalhada.

## A empresa possui sua clientela concentrada principalmente na região sul, seguida pela região nordeste e sudeste, devido à proximidade entre as regiões sul e sudeste, é possível afirmar que a densidade de clientes está direcionada para o sul do país. No entanto, é importante ressaltar que ainda há mais clientes no nordeste do que no sudeste.

| Index | Estado | Contagem |
|---|---|---|
| 0 | BA | 1 |
| 1 | PB | 2 |
| 2 | PR | 1 |
| 3 | RJ | 1 |
| 4 | RS | 1 |
| 5 | SC | 2 |
| 6 | SP | 1 |

Nesse caso, a coluna de 'Contagem' representa o número de clientes, logo, a tabela mostra a quantidade de clientes por Estado.
---

![alt text](https://github.com/Gaba034/desafio-data-analytics/blob/main/graphs/ClientsState.png?raw=true)

---
## A quantidade de produtos vendidos para a região sul é superior às outras regiões, e os estados que mais compraram em cada região foram:
* * Santa Catarina, com 2241 compras.
* * Paraíba, com 2046 compras.
* * São Paulo, com 1502 compras.
Tendo isso em mente, esse gráfico permite ver a densisade de compras por região nesse período de nove meses.
> Cada região apresenta um aspecto climático diferente, podendo impactar fortemente nas vendas.

| Index | ESTADO | Soma_QUANTIDADE_VENDIDA |
|---|---|---|
| 0 | BA | 604 |
| 1 | PB | 2046 |
| 2 | PR | 855 |
| 3 | RJ | 1212 |
| 4 | RS | 1258 |
| 5 | SC | 2241 |
| 6 | SP | 1502 | 
---

![alt text](https://github.com/Gaba034/desafio-data-analytics/blob/main/graphs/SalesQuantState.png?raw=true)

---
## A região sul apresenta a maior densidade de compras, com um total de 15 compras de volumes variados, seguida, em ordem decrescente, pela região nordeste com 13 compras e a região sudeste com 9 compras, sendo assim é possível extrair quais estados fazem um número de compras maior.
O gráfico abaixo representa os dados:

| Index | ESTADO | Soma_QUANTIDADE_VENDIDA |
|---|---|---|
| 0 | PB | 8 |
| 1 | SC | 7 |
| 2 | SP | 5 |
| 3 | BA | 5 |
| 4 | RS | 5 |
| 5 | RJ | 4 |
| 6 | PR | 2 | 
---

![alt text](https://github.com/Gaba034/desafio-data-analytics/blob/main/graphs/SalesState.png?raw=true)

---
## A clientela mais forte da empresa é mais forte da faixa etária de 43-47 anos, além de possuir clientes entre as faixas de 20-26 anos e 58-61 anos também. Cheguei nesta conclusão me embasando nesse gráfico gerado com as informações fornecidas pelos dados, que posteriormente transformei nesta tabela.

|Index |Faixa Etária|PRODUTO|Count|
|---|---|---|---|
|0|20-29|JARDINAGEM|2|
|1|20-29|LIMPEZA|2|
|2|20-29|MANGUEIRAS|2|
|3|20-29|MAQUINA DE CORTAR GRAMA|2|
|4|20-29|UTILIDADES DOMÉSTICAS|2|
|5|30-39|JARDINAGEM|0|
|6|30-39|LIMPEZA|0|
|7|30-39|MANGUEIRAS|0|
|8|30-39|MAQUINA DE CORTAR GRAMA|0|
|9|30-39|UTILIDADES DOMÉSTICAS|0|
|10|40-49|JARDINAGEM|1|
|11|40-49|LIMPEZA|4|
|12|40-49|MANGUEIRAS|4|
|13|40-49|MAQUINA DE CORTAR GRAMA|4|
|14|40-49|UTILIDADES DOMÉSTICAS|4|
|15|50-59|JARDINAGEM|2|
|16|50-59|LIMPEZA|1|
|17|50-59|MANGUEIRAS|0|
|18|50-59|MAQUINA DE CORTAR GRAMA|0|
|19|50-59|UTILIDADES DOMÉSTICAS|1|
|20|60-69|JARDINAGEM|1|
|21|60-69|LIMPEZA|1|
|22|60-69|MANGUEIRAS|1|
|23|60-69|MAQUINA DE CORTAR GRAMA|1|
|24|60-69|UTILIDADES DOMÉSTICAS|1|

---

![alt text](https://github.com/Gaba034/desafio-data-analytics/blob/main/graphs/ClientsAge.png?raw=true)

---
## O produto mais vendido é o de utilidades domésticas, enquanto os produtos de jardinagem são os menos vendidos. Como pode se perceber no gráfico a seguir, que foi feito usando os dados fornecidos:
Além do gráfico, a tabela a seguir ajuda vizualizar todas as vendas por produto.

|Index|Produto|Vendas|
|---|---|---|
|0|MAQUINA DE CORTAR GRAMA|1850|
|1|MANGUEIRAS|1844|
|2|UTILIDADES DOMÉSTICAS |2372|
|3|LIMPEZA|2119|
|4|JARDINAGEM|1533|
---

![alt text](https://github.com/Gaba034/desafio-data-analytics/blob/main/graphs/ProductSales.png?raw=true)

---
## Durante o primeiro trimestre, a empresa experimentou um período de vendas estável, com variações acima da média. No segundo trimestre, houve uma queda nas vendas, com apenas um mês acima da média. Já no terceiro trimestre, dois meses ficaram abaixo da média e um mês apresentou vendas muito acima da média. Usando o gráfico abaixo como base:
Para auxiliar na legibilidade do gráfico, aqui está uma tabela com todas as vendas por mês.

|Index|Mes|Vendas|
|---|---|---|
|0|Janeiro|1742|
|1|Fevereiro|1201|
|2|Março|1169|
|3|Abril|1252|
|4|Maio|1100|
|5|Junho|51|
|6|Julho|396|
|7|Agosto|2000|
|8|Setembro|807|
---

![alt text](https://github.com/Gaba034/desafio-data-analytics/blob/main/graphs/MonthSales.png?raw=true)

---
## Ao longo desses nove meses, observa-se uma tendência de vendas positiva na região sul, com uma boa aceleração. A região sudeste também apresenta uma tendência positiva, porém com uma aceleração menor do que a do sul. Por outro lado, o nordeste apresenta uma tendência negativa, porém com muitas oscilações, tornando difícil prever um padrão.
### Tabela com os dados de vendas pela data da região sul:
|Index|DATA|QUANTIDADE_VENDIDA|
|---|---|---|
|0|2021-01-05|64|
|1|2021-01-15|488|
|2|2021-01-25|420|
|3|2021-02-04|259|
|4|2021-02-14|387|
|5|2021-03-06|69|
|6|2021-03-16|293|
|7|2021-03-26|89|
|8|2021-07-04|396|
|9|2021-08-03|227|
|10|2021-08-13|446|
|11|2021-08-23|409|
|12|2021-09-02|482|
|13|2021-09-12|325|
---

![alt text](https://github.com/Gaba034/desafio-data-analytics/blob/main/graphs/TrendSouth.png?raw=true)

---
### Tabela com os dados de vendas pela data da região sudeste:
|Index|DATA|QUANTIDADE_VENDIDA|
|---|---|---|
|0 |2021-02-24|302|
|1 |2021-03-06|117|
|2 |2021-03-16|344|
|3 |2021-04-15|292|
|4 |2021-04-25|447|
|5 |2021-05-15|294|
|6 |2021-08-23|918|
---

![alt text](https://github.com/Gaba034/desafio-data-analytics/blob/main/graphs/TrendSoutheast.png?raw=true)

---
### Tabela com os dados de vendas pela data da região nordeste:
|Index|DATA|QUANTIDADE_VENDIDA|
|---|---|---|
|0|2021-01-05|257|
|1|2021-01-15|51|
|2|2021-01-25|462|
|3|2021-02-04|253|
|4|2021-03-16|257|
|5|2021-04-15|51|
|6|2021-04-25|462|
|7|2021-05-05|295|
|8|2021-05-15|403|
|9|2021-05-25|108|
|10|2021-06-14|26|
|11 |2021-06-24|25|
---

![alt text](https://github.com/Gaba034/desafio-data-analytics/blob/main/graphs/TrendNortheast.png?raw=true)

---
## Em relação à faixa etária e aos produtos, foi observado que algumas faixas etárias não demonstraram interesse em determinados tipos de produtos. Por exemplo, a faixa etária de 50-59 anos não adquiriu produtos como mangueiras e máquinas de cortar grama. A mesma tabela usada anteriormente pode servir para a vizualização.

|Index |Faixa Etária|PRODUTO|Count|
|---|---|---|---|
|0|20-29|JARDINAGEM|2|
|1|20-29|LIMPEZA|2|
|2|20-29|MANGUEIRAS|2|
|3|20-29|MAQUINA DE CORTAR GRAMA|2|
|4|20-29|UTILIDADES DOMÉSTICAS|2|
|5|30-39|JARDINAGEM|0|
|6|30-39|LIMPEZA|0|
|7|30-39|MANGUEIRAS|0|
|8|30-39|MAQUINA DE CORTAR GRAMA|0|
|9|30-39|UTILIDADES DOMÉSTICAS|0|
|10|40-49|JARDINAGEM|1|
|11|40-49|LIMPEZA|4|
|12|40-49|MANGUEIRAS|4|
|13|40-49|MAQUINA DE CORTAR GRAMA|4|
|14|40-49|UTILIDADES DOMÉSTICAS|4|
|15|50-59|JARDINAGEM|2|
|16|50-59|LIMPEZA|1|
|17|50-59|MANGUEIRAS|0|
|18|50-59|MAQUINA DE CORTAR GRAMA|0|
|19|50-59|UTILIDADES DOMÉSTICAS|1|
|20|60-69|JARDINAGEM|1|
|21|60-69|LIMPEZA|1|
|22|60-69|MANGUEIRAS|1|
|23|60-69|MAQUINA DE CORTAR GRAMA|1|
|24|60-69|UTILIDADES DOMÉSTICAS|1|

---

![alt text](https://github.com/Gaba034/desafio-data-analytics/blob/main/graphs/Dispersão.png?raw=true)

---
# Análise de Vendas:
Aqui estão alguns insights para a empresa:

* Planejamento sazonal: Como seus produtos estão relacionados à casa e ao jardim, é natural que as vendas sofram variações sazonais, com queda nos meses mais frios e aumento com a chegada da primavera. É importante prestar atenção especial ao planejamento para atender à demanda sazonal e garantir estoques adequados durante esses períodos.

* Variações regionais: Devido ao tamanho e diversidade climática do país, a empresa deve estar atenta às diferenças sazonais de cada região, pois isso pode impactar significativamente as vendas em cada região. Como observado nos gráficos de tendência, a região sudeste experimentou um salto nas compras, de 200 para 900, enquanto a região nordeste apresentou uma tendência de queda. Essas variações regionais devem ser consideradas nas estratégias de marketing e distribuição.

* Segmentação por faixa etária: Embora o público em geral não seja uma grande preocupação, já que os produtos relacionados à casa têm um impacto distribuído em adultos, é importante analisar o comportamento de compra de diferentes faixas etárias. Os gráficos indicam que a faixa etária de 20-29 anos apresenta um padrão de compra distribuído. A faixa etária de 40-49 anos mostra pouco interesse em produtos relacionados à jardinagem, mas possui boas compras relacionadas aos outros produtos. A faixa etária de 50-59 anos demonstra pouco interesse geral nos produtos, mas mostra uma preferência por produtos de jardinagem. Já a faixa etária de 60-69 anos compra os produtos de forma equilibrada. Essas informações podem ser usadas para ajustar a comunicação e estratégias de venda, personalizando a abordagem de acordo com as preferências de cada faixa etária.

# Estratégias de Marketing:

* Segmentação regional: Dado que a região sul concentra a maior parte da clientela da empresa, é importante direcionar esforços de marketing para expandir a presença nas regiões nordeste e sudeste. Isso pode ser feito por meio de campanhas publicitárias segmentadas, presença em feiras e eventos regionais, parcerias com varejistas locais e ações promocionais específicas para cada região.

* Aumento da base de clientes: A expansão para novas regiões significa acessar uma base de clientes maior. Isso pode resultar em um aumento significativo no número de clientes e, consequentemente, em mais fontes de lucro. A diversificação geográfica reduzirá a dependência de um único mercado e tornará o negócio mais resiliente a flutuações econômicas regionais.

* Aprendizado e inovação: Cada nova região trará aprendizados valiosos e insights sobre diferentes mercados e clientes. Essas informações podem ser aplicadas para melhorar sua estratégia geral e impulsionar a inovação dentro da empresa.

* Promoções sazonais: Aproveite as variações sazonais nas vendas, com ênfase nos meses de maior demanda, como a primavera e o verão, para promover os produtos relacionados à casa e ao jardim. Ofereça descontos, pacotes promocionais ou brindes para incentivar as compras nesses períodos.

* Personalização de comunicação: Utilize a segmentação por faixa etária para personalizar a comunicação e as estratégias de venda. Crie mensagens e abordagens que sejam relevantes para cada grupo etário, destacando os benefícios específicos dos produtos para suas necessidades e preferências.

* Parcerias estratégicas: Estabeleça parcerias com influenciadores digitais, blogueiros ou especialistas em decoração de casa e jardinagem, que possam promover os produtos da empresa por meio de análises, recomendações e tutoriais. Essas parcerias podem ajudar a aumentar a visibilidade da marca e alcançar um público mais amplo.

* Marketing digital: Invista em marketing digital para aumentar a visibilidade da empresa e impulsionar as vendas. Utilize estratégias de SEO (otimização de mecanismos de busca) para melhorar o posicionamento do site nos resultados de pesquisa, faça uso de redes sociais para interagir com os clientes, compartilhar conteúdo relevante e promover as ofertas da empresa.

* Programa de fidelidade: Implemente um programa de fidelidade para incentivar compras repetidas e recompensar os clientes fiéis. Ofereça descontos exclusivos, brindes ou acesso antecipado a novos produtos como forma de recompensar a lealdade dos clientes.

* Acompanhamento pós-venda: Mantenha um relacionamento próximo com os clientes, enviando e-mails personalizados de acompanhamento pós-venda, solicitando feedback e oferecendo suporte adicional. Isso demonstrará o cuidado da empresa com a satisfação do cliente e ajudará a construir uma reputação positiva.

# Limitações:

* Quantidade limitada de dados: Com uma quantidade limitada de dados, é difícil obter uma análise precisa e completa. Uma amostra pequena pode não ser representativa o suficiente para tirar conclusões generalizadas ou identificar tendências confiáveis.

* Falta de amplitude dos dados: Um período de um ano pode não ser suficiente para capturar flutuações sazonais ou ciclos de longo prazo. Para obter uma compreensão mais completa do desempenho, seria necessário analisar um período mais longo de dados, levando em consideração possíveis variações ao longo do tempo.

* Falta de contexto: A análise de dados sozinha não é suficiente para fornecer recomendações eficazes. É essencial conhecer as estratégias e os objetivos da empresa para avaliar adequadamente o desempenho e identificar possíveis melhorias. Sem esse contexto, é difícil oferecer insights valiosos ou sugestões específicas.

# Implicações: 

Em conclusão, com base na análise realizada, a empresa tem uma oportunidade significativa de aprimorar suas estratégias de marketing. Adaptar-se às questões sazonais, considerar as diferenças climáticas regionais, segmentar a comunicação por faixa etária e expandir a presença em regiões específicas são passos importantes para impulsionar o crescimento do negócio.
Ao planejar cuidadosamente campanhas sazonais, personalizar a comunicação e utilizar estratégias de marketing digital, a empresa poderá alcançar um público mais amplo, engajar clientes em potencial e fortalecer o relacionamento com os clientes existentes. Além disso, a implementação de um programa de fidelidade pode estimular os clientes, gerando vendas repetidas e promovendo a construção de relacionamentos duradouros.
No entanto, é crucial ter em mente que essas recomendações são baseadas em uma análise limitada de dados e que cada empresa possui seu próprio contexto específico. Portanto, é essencial conduzir pesquisas adicionais, adaptar as estratégias às necessidades e características da empresa e monitorar os resultados para obter um crescimento sustentável e bem-sucedido no mercado.