Jessica Finardi dos Santos
Análise de Dados – Turma V2

# Análise de Dados - Dataset Varejo
## Limpeza e Tratamento dos Dados
- Importação das bibliotecas Pandas e NumPy.
- Leitura do dataset.
- Identificação de valores nulos e duplicados.  
Através da análise foi verificado um total de 830.000 linhas e 14 colunas. Encontradas 4 colunas que estavam com todas as linhas nulas e 96.553 registros com duplicatas.  
Criada a cópia do dataset, para iniciar o tratamento dos dados, onde optei por excluir as colunas unnamed:10, unnamed:11, unnamed:12, unnamed:13, visto que todas as linhas referentes a elas estavam vazias, e esses dados não agregavam em nada na exploração. Foi feita a análise das linhas duplicadas e feito a remoção das mesmas, mantendo a primeira ocorrência. Haviam categorias e produtos com ‘#N/D’ onde na coluna ‘PR_CAT’ foi optado por substituir por ‘Sem Categoria’ e na coluna ‘PR_NOME’ por ‘Produto Não Informado’. Feita a conversão da coluna ‘DATA’ para datetime, muitas datas ainda ficaram como ‘NaT’ mas mantive assim, visto que não utilizei elas para responder as perguntas de negócio. 
## Verificada as estatísticas: 
- Média
- Mediana
- Moda
- Desvio padrão
- Quartis
## Perguntas de negócios e análises: 
### Quais são os produtos mais consumidos por cada gênero?
### Alguma das categorias é mais vendida num gênero em específico?
Para responder essa questão foi feito o agrupamento por gênero e quantidade de compras em cada segmento, observado que a categoria mais vendida é a de alimentos, seguida dos produtos de higiene e limpeza que seguem parâmetros parecidos pra ambos os gêneros. Em todas as categorias não temos valores discrepantes comparando uma com as outras, mas é possível verificar que ainda assim o gênero feminino é o que mais realiza compras em todos os segmentos.
### A quantidade de filhos pode estar influenciando no comportamento de compras dos clientes?
### Clientes com mais filhos consomem mais alguma categoria em específico?
Feito o agrupamento por quantidade de filhos versus quantidade comprada em cada segmento. Nessa análise observa-se que independente do número de filhos, a categoria de alimentação lidera no segmento, representando mais da metade das compras. É possível verificar também que o grupo sem filhos lidera as compras em todos os segmentos, o que poderia significar que temos mais clientes sem filhos no dataset. Nos grupos com filhos observa-se que as categorias de higiene e limpeza seguem valores parecidos mostrando um comportamento de consumo mais ligado a rotina do dia-a-dia. Independentemente da quantidade filhos observou-se um padrão parecido de gastos com pets, indicando que possuir filhos não estaria impactando nesse segmento.
### Quais são os 10 produtos mais vendidos?
Observa-se através do top 10 em vendas, que a venda dos produtos é bastante diversificada, sendo desde alimentos à produtos de higiene e limpeza. O que demonstra que a empresa tem uma boa saída de produtos em todas as categorias. O produto que mais se destaca, tendo vendido praticamente mais que o dobro do segundo colocado, é o presunto cozido. Isso demonstra que é um item de compra recorrente dos clientes. A partir do segundo colocado temos valores de vendas bem próximos nas demais categorias, mostrando quantidade de vendas parecidas nesses segmentos.
