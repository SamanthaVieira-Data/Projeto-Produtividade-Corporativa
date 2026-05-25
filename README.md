# 📊 Corporate Productivity Analysis | Análise de Produtividade Corporativa

> **Note:** This project was originally developed in Portuguese. You can find the full English documentation below, followed by the original Portuguese version.

[English Version](#english-version) | [Versão em Português](#versão-em-português)

---

## English Version

### 📋 About the Project
This project delivers an **end-to-end analysis**, covering the complete data lifecycle from initial extraction to the final solution delivery. The development unifies Python's processing power with Power BI's visual excellence. The entire framework was designed following UX Design principles and the Inverted Pyramid logic, ensuring that the Executive Summary serves as the strategic starting point, followed by technical and operational details.

### 🏗️ Methodology and Data Governance

A key differentiator of this project was the data reconciliation stage, ensuring information security before building any visuals.

* **Database Integrity:** The total revenue of R$ 5.52M was validated through a cross-check between Python and Power BI. The exact match between both platforms proves there are no errors in the data integration or business rules application.
* **💡 Validation Strategy:** The development adopted a dual analytical check. Python was used for initial mapping and extracting preliminary business metrics, while Power Query within Power BI replicated this exact calculation and structuring logic to guarantee data consistency and flawless dashboard filter behavior.
* **Scalability and Flexibility:** Raw table integration was structured in Python using the `.merge(how='left')` function, which provides flexibility when connecting databases, combined with `.groupby().size()` to ensure model scalability, mapping and grouping all records without data loss before the final report load.

### 📈 Dashboard Visualization

#### 1. Executive Summary & Strategic Drivers
The report's landing page features the primary Key Performance Indicators (KPIs) and acts as the board's decision-making panel, highlighting two major strategic drivers for corporate growth:

* **Commercial Efficiency Strategy:** Identifying productivity gaps across teams led to a proposed cross-training program between the Administrative and Commercial departments. This allows process sharing to boost contract volume by 30% without incurring new hiring costs.
* **Strategic Insight:** The analysis revealed that fully integrating the remaining 15 professionals has the potential to increase annual revenue from R$ 5.52 Million to approximately R$ 6.6 Million, representing a 15% boost in overall productivity.

![Executive Summary](1_sumario_executivo.png)

#### 2. Sales Performance
This view details global revenue indicators and identifies the organization's Top Performers to guide training strategies.

* **Talent Benchmark:** The mapping identified an Operations department employee leading the Top Performers with 6 closed contracts, establishing an internal high-performance benchmark to model the cross-training program.
* **Efficiency Indicator:** Monitoring set the Global Monthly Average Ticket at R$ 2,502.56, serving as a control metric to evaluate the profitability of new contracts signed across sectors.

![Sales Performance](2_performance_de_vendas.png)

#### 3. Department View & Productivity
These views present comparative charts of the Average Ticket per department and correlate contract volume with the total headcount.

* **Technical Note:** In Power BI, a decimal scale showing an average of 2.39 contracts per employee was selected to simplify executive reading, ensuring quick comprehension of individual productivity levels without visual noise.

![Department View](3_visao_por_area.png)

![Productivity](4_produtividade.png)

### 🛠️ Technologies and Data Sources

* **Data Sources:** Integration of multiple datasets in `.csv` format for Employee and Client databases, and `.xlsx` for the Provided Services log.
* **Python (Pandas & Matplotlib):** Execution of the entire ETL process, handling distinct data types, and performing exploratory visual analysis to validate business hypotheses.
* **Power BI:** Relational data modeling, development of calculated measures using DAX, and interactive dashboard interface design.

> **Note:** The "Laboratory" tab was kept as a hidden page within the `.pbix` file for technical validation and future metric expansions.

## ⚠️ Disclaimer

I declare that all data used in this Revenue and Operational Performance Analysis project consists of **simulated and fictitious** information created solely for academic purposes to demonstrate technical skills in Python, Pandas, and Business Intelligence. 

These records **do not represent real, sensitive, or confidential information** of any organization. Therefore, the insights and recommendations generated are based entirely on this hypothetical dataset.

---

## Versão em Português

# Análise de Faturamento e Desempenho Operacional de uma Empresa

### 📋 Sobre o Projeto
Este projeto realiza uma **análise end-to-end** por envolver o ciclo completo de análise de dados, desde a extração inicial até a entrega da solução final. O desenvolvimento unificou o poder de processamento do Python com a excelência visual do Power BI. Toda a estrutura foi desenhada seguindo os princípios de UX Design e a lógica da Pirâmide Invertida de modo que o Sumário Executivo atue como o ponto de partida estratégico e o detalhamento técnico e operacional surja na sequência.

### 🏗️ Metodologia e Governança de Dados

Um grande diferencial deste projeto foi a etapa de conciliação para garantir a segurança das informações antes da construção dos visuais.

* **Integridade das Bases:** O faturamento total de R$ 5,52 Mi foi validado por meio de uma checagem cruzada entre Python e Power BI de modo que a concordância dos valores comprova a ausência de erros no cruzamento das fontes e a aplicação correta das regras de negócio.
* **💡 Estratégia de Validação:** O desenvolvimento adotou uma dupla checagem analítica utilizando tanto o Python para realizar o mapeamento inicial e extrair as primeiras conclusões e métricas do negócio quanto o Power Query dentro do Power BI, replicando essa mesma lógica de cálculo e estruturação para assegurar a consistência dos dados e o perfeito funcionamento dos filtros do dashboard.
* **Escalabilidade e Flexibilidade:** A junção das tabelas brutas foi estruturada em Python por meio da função `.merge(how='left')` que confere flexibilidade na conexão das bases e do `.groupby().size()` que garante a escalabilidade do modelo permitindo mapear e agrupar a totalidade dos registros sem o risco de perda de informações antes da carga final no relatório.

### 📈 Visualização do Dashboard

#### 1. Sumário Executivo & Direcionais Estratégicos
A página inicial do relatório apresenta os principais indicadores de desempenho e funciona como o painel de tomada de decisão da diretoria, revelando, sobretudo, dois grandes direcionadores estratégicos para o crescimento da empresa.

* **Estratégia de Eficiência Comercial:** A identificação do desvio de produtividade entre as equipes levou à proposta de um programa de *cross-training* entre as áreas Administrativa e Comercial permitindo o compartilhamento de processos para alavancar em 30% o volume de contratos sem gerar novos custos de contratação.
* **Insight Estratégico:** A análise identificou que a integração total dos 15 profissionais restantes tem o potencial de elevar a receita anual da empresa de R$ 5,52 Milhões para aproximadamente R$ 6,6 Milhões representando um incremento de 15% na produtividade geral.

![Sumário Executivo](1_sumario_executivo.png)

#### 2. Performance de Vendas
Esta visão detalha os indicadores globais de faturamento e identifica os Top Performers da organização para nortear as estratégias de treinamento.

* **Benchmark de Talento:** O mapeamento identificou o colaborador do setor de Operações na liderança dos Top Performers com 6 contratos fechados, o que estabelece um referencial interno de alta performance para servir de modelo ao programa de *cross-training*.
* **Indicador de Eficiência:** O monitoramento fixou o Ticket Médio Mensal Global em R$ 2.502,56 servindo como métrica de controle para avaliar a rentabilidade dos novos contratos assinados em cada setor.

![Performance de Vendas](2_performance_de_vendas.png)

#### 3. Visão por Área & Produtividade
Estas visões apresentam gráficos comparativos de Ticket Médio por setor e correlacionam o volume de contratos com o quadro total de funcionários.

* **Nota Técnica:** No Power BI, optou-se pela utilização da escala decimal com a média de 2,39 contratos por funcionário para simplificar a leitura executiva e garantir a rápida compreensão do nível de produtividade por indivíduo de forma direta e sem ruídos visuais.

![Visão por Área](3_visao_por_area.png)

![Produtividade](4_produtividade.png)

### 🛠️ Tecnologias e Origem dos Dados

* **Fontes de Dados:** Integração de múltiplos datasets em formatos `.csv` para as bases de Funcionários e Clientes e `.xlsx` para a base de Serviços Prestados.
* **Python (Pandas & Matplotlib):** Execução de todo o processo de ETL com o tratamento de tipos de dados distintos e análise visual exploratória para a validação das hipóteses de negócio.
* **Power BI:** Construção da modelagem relacional de dados, criação de medidas calculadas em DAX e desenvolvimento do design dos dashboards interativos.

> **Obs:** A aba Laboratório foi mantida como uma página oculta no arquivo `.pbix` para fins de validação técnica e futuras expansões de métricas.

## ⚠️ Disclaimer

Declaro que todos os dados utilizados neste projeto de Análise de Faturamento e Desempenho Operacional são constituídos por informações **simuladas e fictícias** criadas exclusivamente para fins acadêmicos com o objetivo de demonstrar habilidades técnicas em Python, Pandas e Business Intelligence.

Estes registros **não representam informações reais, sigilosas ou confidenciais** de nenhuma organização de modo que as conclusões e recomendações geradas são baseadas unicamente neste conjunto de dados hipotéticos.