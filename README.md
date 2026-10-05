# SamuelScotti_Projetoavaliativo_Modulo01_SamuelScotti_T3_Dados_BI

# Projeto Avaliativo - Visualização de Dados e BI

**Aluno:** Samuel Scotti
**Turma:** T3

## Objetivo do Trabalho
Este projeto tem como objetivo analisar os dados de RH de uma empresa utilizando SQL para extração e Python para análise exploratória. O foco é entender a distribuição de salários, a relação entre cargos e departamentos, e os padrões de remuneração por região.

## Tabelas Utilizadas
* **EMPLOYEES:** Contém os dados principais dos colaboradores, como ID, nome e salário.
* **DEPARTMENTS:** Contém os nomes dos departamentos e a sua localização.
* **JOBS:** Contém os títulos dos cargos.
* **LOCATIONS, COUNTRIES, REGIONS:** Tabelas utilizadas para mapear a distribuição geográfica dos colaboradores.

## Consultas SQL
1. **`query_1.sql`:** Utiliza `LEFT JOIN` para relacionar colaboradores, departamentos e cargos, filtrando apenas departamentos válidos (`WHERE DEPARTMENT_ID IS NOT NULL`).
2. **`query_2.sql`:** Relaciona colaboradores à sua localização geográfica completa, garantindo que a região não é nula (`WHERE REGION_NAME IS NOT NULL`).

## Análise em Python
A análise exploratória foi realizada num caderno Jupyter (`analise_eda.ipynb`) utilizando as bibliotecas `pandas`, `matplotlib` e `seaborn`. Foram calculadas estatísticas descritivas (média, mediana, mínimo e máximo) da remuneração e geradas visualizações gráficas para facilitar o entendimento da distribuição salarial.

## Principais Resultados Encontrados
* **Estatísticas Salariais:** A média salarial da empresa é de $ 6456.75 e a mediana é de $ 6150.00. O salário mínimo registado é de $ 2100.00 e o máximo de $ 24000.00.
* **Distribuição (Histograma):** A análise revela que a grande maioria dos colaboradores da empresa concentra-se na faixa salarial mais baixa, recebendo entre $ 2.000 e $ 5.000. A distribuição é fortemente assimétrica, mostrando que apenas uma pequena minoria de funcionários recebe salários superiores a $ 10.000.
* **Departamentos (Boxplot):** Fica claro que o departamento Executive detém as remunerações mais elevadas e discrepantes do resto da empresa, acima dos $ 15.000. Em contrapartida, departamentos operacionais como Purchasing e Shipping apresentam os salários mais baixos e com a menor variação entre os seus funcionários. Adicionalmente, o departamento de Sales é o que apresenta a maior amplitude salarial, com valores muito variados entre a sua equipa.

## Como Executar o Projeto
**Pré-requisitos:** Python 3 instalado.
1. Clone o repositório: ‘git clone https://github.com/SamuelScotti/SamuelScotti_Projetoavaliativo_Modulo01_SamuelScotti_T3_Dados_BI.git'
2. Instale as bibliotecas necessárias: `pip install pandas matplotlib seaborn`
3. Abra o ficheiro `analise_eda.ipynb` num editor compatível e execute as células sequencialmente.

## Sugestões de Melhoria
Recomenda-se a inclusão de uma coluna categórica de "Gênero" na tabela EMPLOYEES. Isso permitiria investigar possíveis disparidades salariais entre homens e mulheres e analisar a representatividade de gênero em cargos de alta liderança.

## Vídeo de Apresentação
https://drive.google.com/file/d/1JoBd71-Vw2kRPxZHmOomojhu4GQh2Wi3/view?usp=sharing