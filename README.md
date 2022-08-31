# Projeto Sentiment Analysis - Mosteiro dos Jerônimos

## Descrição Inicial

Durante o projeto, o meu objetivo foi passar pelas etapas de extração dos dados, de entendimento do problema, ideação da solução, análise dos fatores que poderiam influenciar e, por fim, a etapa de Análise de Sentimentos. O foco principal é destrinchar os comentários coletados no site, em inglês, do TripAdvisor sobre o Mosteiro dos Jerônimos, importante ponto turístico da cidade de Lisboa. A partir disso, buscar insights atráves dos textos e definir se eram positivos ou negativos, dado o que estava sendo dito, após o pré-processamento do texto. Alguns questionamentos inicias importantes são:

- Há majoritariamente comentários positivos ou negativos?

- Dentre os comentários positivos, quais as palavras ou ideais que mais se destacam?

- Como nos comentários positivos, dentre os comentários negativos, quais as palavras ou ideias que mais se destacam?

- O que poderia ser feito para melhorar os pontos negativos abordados?

Ao final do projeto é entregue uma lista de palavras e suas combinações, tanto positivas quanto negativas, além de um WordCloud e uma possível solução dado o problema encontrado.

Para que a solução fosse entregue, foram utilizadas algumas tecnologias na Análise de Dados e Natural Language Processing (NLP), tais como **Pandas, Matplotlib, Seaborn, NLTK, TextBlob, Pattern, WordCloud, Scrapy**.

Antes de iniciar toda a análise, a proposta do projeto foi escolhida e assim se buscou extrair esses dados do TripAdvisor com o framewordk **Scrapy**, gerando uma *spider* que passou por todas as páginas dos comentários relacionado ao Mosteiro dos Jerônimos e armazenou tudo em um arquivo .csv.

Para as etapas de Análise e Manipulação de dados foi utilizado o **Pandas**. Durante o cerne do projeto, foram utilizadas as bibliotecas **NLTK, TextBlob, Pattern**, responsáveis por pré-processarem o texto, analisar os sentimentos contidos nas sentenças e o entendimento, a partir dos bigrams e trigrams, um pouco mais do contexto nos quais as principais palavras estão inseridas. Para melhor representar esses conjuntos de palavras, de maneira mais visual, foram gerados Word Clouds com a bibloteca **WordCloud**. Por fim, mas não menos importante, foram criados gráficos utilizando **Matplotlib e Seaborn**. 

#Etapas do Projeto (Após extração):

**Descrição das Variáveis**

autor_comentarios  - criador do comentário

corpo_comentarios  - corpo de comentário escrito

data_comentarios   - data que foi emitido o comentário

título_comentarios - título dado pelo criado do comentário

#
**Durante a etapa de Análise e de NLP foram descobertos diversos insights**

- Analisando-se os dados, há uma quantidade expressivamente maior de comentários positivos a negativos ou neutro

- O nível de subjetividade é bem maior ao de objetividade, o que já era esperado se tendo a base de dados do TripAdvisor e com isso a opinião das pessoas

- É possível notar um grande aumento dentre 2014 a 2017, com queda vertiginosa a partir de 2018, voltando em 2020 a números tão baixos quanto no período antes do crescimento em 2014.

- Esse padrão é percebido tanto nos comentários positivos quanto negativos e teria que ser melhor investigado para saber as mudanças, seja no TripAdvisor ou no Mosteiro dos Jerônimos, nesse período

- Interessante destacar que dos comentários positivos, é demonstrado interesse pela arquitetura do local, pela beleza dele e pelos pontos turísticos nas redondezas, como a Torre de Belém e o Pastel de Belém.

- Com relação aos comentários negativos, destacam-se as longas filas e o guichê de compra de ingressos.

## Conclusão

Com a análise, pode se inferir problemas quanto ao gerencimento da venda de tickets e a capacidade de pessoas, criando filas que incomodam os clientes que buscam visitar o local e que se encantam com o mesmo. Como possíveis medidas, seria interessante avaliar o sistema de venda de tickets, o tempo atual de espera (nos cenários de baixa e alta temporada) e buscar alternativas de implementação para redução do tempo de espera, como um FastPass (similiar ao existente na Disney) comprado a priori para agilizar o processo e melhorar a experiência

Logo, através desse projeto pude passar, desde a extração de dados no TripAdvisor, passando pela análise dos possíveis objetivos até o entendimento de alguns problemas e possíveis soluções, utilizando de técnicas de manipulação de dados e de NLP, como a **Análise de Sentimentos (Sentiment Analysis)**.

Como proposta de melhoria futura, a extração de dados de outras fontes para ampliar a gama de resultados possíveis, automatização do processo de ETL e de manipulação dos dados. 


