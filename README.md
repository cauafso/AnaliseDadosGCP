# Projeto Final Google Cloud Data Analytics
Projeto final do curso Google Cloud Data Analytics

## Cenário

A TheLook Fintech é uma nova empresa de tecnologia financeira que faz empréstimos a proprietários de lojas on-line independentes que precisam de recursos financeiros para adquirir estoque. A missão da empresa é mudar a forma como as pessoas têm acesso a empréstimos para expandir os negócios. Minha primeira atribuição é desenvolver e implementar um plano para ajudar o departamento financeiro a usar os dados de forma eficaz com objetivo de acompanhar a performance e o crescimento da TheLook. Três questões de negócios foram identificadas durante uma reunião com o líder do departamento financeiro.

São elas:

Como monitorar melhor nosso fluxo de caixa para garantir que o volume dos empréstimos liberados a cada mês não supere o montante que entra no caixa?
Como identificar os principais motivos que levam os clientes a pegar empréstimos conosco?
Como rastrear os locais onde os mutuários estavam quando contrataram os empréstimos?

Minha segunda etapa é desenvolver um dashboard para ajudar a equipe a aproveitar ao máximo os dados de integridade dos empréstimos e ter acesso rápido e fácil às informações de que precisam.

Foram identificadas quatro perguntas de negócios importantes que sempre surgem quando a equipe discute a integridade dos empréstimos.

São elas:

Qual é o valor total pendente de todos os empréstimos?
Qual é a porcentagem de empréstimos pendentes em cada categoria de status?
Quais estados têm a maior quantidade de empréstimos pendentes?
Quais clientes já quitaram a própria casa e têm empréstimos vigentes?

## Primeira Etapa
### Coletar, processar e armazenar dados no BigQuery

**Processo de análise da Primeira Etapa**

1. Analisei o conjunto de dados para descobrir quais variáveis utilizar na análise.
2. Importei um arquivo CSV, contendo informações sobre estados, regiões e sub_regiões dos EUA, do Cloud Storage para o BigQuery, criando uma nova tabela chamada state_region.
3. Realizei a junção das tabelas empréstimos(Loan) e a tabela sobre regiões(state_region).
4. Realizei uma query para retornar linhas únicas dos motivos de empréstimos dos clientes.
5. Realizei uma query para retornar o valor total dos empréstimos por ano.
6. Realizei uma query para retornar o total de empréstimos feitos por ano.
  
Atráves dessa análise temos o matérial necessário para responder as perguntas de negócio da primeira etapa.

## Segunda Etapa
### Analisar e ativar dados com o Looker Enterprise

**Processo de criação do Dashboard**

1. Criei uma visualização de visão geral sobre o valor pendente de empréstimos.
2. Criei um gráfico de pizza para representar os dados de porcentagem, para termos um dimensão do todo.
3. Optei por um gráfico de barras verticais para a visualização dos estados com maior quantidade de empréstimos, para termos a imagem de ranking.
4. Optei em criar uma tabela para demonstrar os dados requeridos dos clientes.




