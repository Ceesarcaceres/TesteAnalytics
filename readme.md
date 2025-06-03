Relatório Técnico

Utilizei python para fazer todo o processo ETL, com as bibliotecas pandas e numpy
para leitura e tratamento de dados, json para transformar o campo metadata na tabela web_events
em coluna e linha, e unicodedata para fazer um tratamento para remover acentos em emails e nomes 
que estavam quebrados.

Realizei tratamento de dados nas colunas de datas das tabelas, estado que estavam foram do padrão,
alterei o endereço que estavam com ',' como separador para '-', para deixar padronizado a tabela.
Transformei o valor total da compra na tabela de orders para padronizar de acordo com cada tipo de moeda,
definindo milhar como '.' e decimal ',' para BRL e outras moedas como ',' para milhar e decimal como '.'
Existiam alguns emails com acento, no qual tratei e retirei os acentos dos emails.

Desafios

Não identifiquei desafios muito difícieis de resolver, acredito que foram mais identificar alguns
dados incorretos, como o e-mail com acento e também os emails repetitivos, pois como eram em poucos 
casos, tive que analisar bem as bases de dados.
Após identificar fiz as limpezas necessárias e os erros foram resolvidos.

Exemplos:

Metadata JSON:
Antes:

![image](https://github.com/user-attachments/assets/50b62526-7590-4e45-95db-61b9d78c640b)

Depois:

![image](https://github.com/user-attachments/assets/ff97ded0-4039-44c4-8482-2337871b4e45)

Endereço (para deixar padronizado):
Antes:

![image](https://github.com/user-attachments/assets/70495d3c-765f-41bd-b450-3dbfb6b86a83)

Depois:

![image](https://github.com/user-attachments/assets/972d3bfa-f531-4a8a-806d-567743d33313)

order_date e amount:
Antes:

![image](https://github.com/user-attachments/assets/70649e4c-6813-4ba8-8e49-58f6a9fb4112)

Depois:

![image](https://github.com/user-attachments/assets/046b0f25-4623-4bc7-bddb-3ca18da558b4)

registration_date, birth_date e state:

Antes:

![image](https://github.com/user-attachments/assets/e2316838-237b-413a-bca0-b7e59039786a)

Depois:

