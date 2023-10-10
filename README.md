# Descrição

O objetivo desse projeto é identificar padrões nos dados da loja online Ice Games.Padrões que a equipe de vendas e marketing possa usar para elaborar estratégias publicitárias e de venda. A loja Ice vende para o mundo todo, sendo assim temos dados amostrais de populações diferentes. Temos as avaliações de usuários e especialistas, gêneros e plataformas (por exemplo, Xbox ou PlayStation).

Os dados disponíveis são de até 2016 a estratégia é identificar os padrões para as vendas de 2017. 

O conjunto de dados também contém a abreviatura ESRB. O Entertainment Software Rating Board avalia o conteúdo de um jogo e atribui uma classificação etária, como Adolescente ou Maduro.

## Estrutura do projeto

**Passo 1. Abertura e análise exploratória inicial.**  

- Caminho do arquivo:


`*/datasets/games.csv*` . [Download dataset](https://practicum-content.s3.us-west-1.amazonaws.com/datasets/games.csv)


- Com o arquivo carregado, foi analisado uma amostra dos dados e as informações gerais. Para identificar erros .

**Passo 2. Preparar os dados**

Foram identificados  problemas nos dados, que precisaram ser tratados, para a continuidade do projeto. Os ajustes realizados foram: 

- Substituir os nomes das colunas (transformar tudo em minúsculos).
- Converta os dados para os tipos certos.
- Tratar valores ausentes explícitos e não explícitos (valores “tbd” na coluna de classificação)
- Foi calculado o total de vendas (a soma das vendas em todas as regiões) para cada jogo e colocado os valores em uma coluna separada.

**Passo 3. Análise dos dados**

- Primeiro foi olhado os lançamentos de jogos por período de ano.
- Separei e criei um histograma para as plataformas que mais venderam no passado e não vendem mais, assim foi possível estimar a média de vida útil das plataformas , quanto tempo demora para as novas plataformas aparecerem e para as velhas desaparecerem  .
- Para construir um modelo analítico para 2017, decidi usar apenas os dados de 2012 a 2016.
- Foi observado como as vendes variam de plataforma para plataforma
- As analises seguinte foram feitas para responder as seguintes questões  :
    - Quais plataformas estão liderando em vendas?
    - Quais estão crescendo ou diminuindo?
    - As diferenças nas vendas são significativas?
    - Quais plataformas com o maior potencialmente lucrativas.
    - E quanto às vendas médias em várias plataformas?
    - As avaliações dos usuários e críticos afetam as vendas de uma plataforma popular ?
    - Quais os gêneros mais lucrativos?
    - Pode generalizar sobre gêneros com vendas altas e baixas?
    

**Passo 4. Criar um perfil de usuário para cada região**

Para cada região (AN, UE, JP), foi determinado:

- As cinco plataformas principais. Descrito as variações das suas quotas de mercado de região para região.
- Os cinco principais gêneros e quais suas diferenças.
- As classificações do ESRB afetam as vendas em regiões individuais?

**Passo 5. Teste de hipóteses:**

— As classificações médias dos usuários das plataformas Xbox One e PC são as mesmas.

— As classificações médias de usuários para os gêneros Action (ação) e Sports (esportes) são diferentes.

O valor do limiar Alfa foi de 5%.

**Passo 6.  Conclusão geral**

### Descrição de dados

—*Name* (nome)

—*Platform* (plataforma)

—*Year_of_Release* (Ano de lançamento)

—*Genre*(gênero)

—*NA_sales* (vendas norte-americanas em milhões de USD)

—*EU_sales* (vendas na Europa em milhões de USD)

—*JP_sales* (vendas no Japão em milhões de USD)

—*Other_sales* (vendas em outros países em em milhões de USD)

—*Critic_Score* - (Pontuação crítica) (máximo de 100)

—*User_Score* -  (Pontuação do usuário) (máximo de 10)

—*Classificação* (ESRB)

Os dados de 2016 estão incompletos.
