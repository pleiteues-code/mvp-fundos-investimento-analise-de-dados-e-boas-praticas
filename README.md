# 📊 MVP – Análise de Fundos de Investimento

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/pleiteues-code/mvp-fundos-investimento-analise-de-dados-e-boas-praticas/blob/main/MVP_Fundos_Investimento_Paulo_Ricardo_Marques_Leite.ipynb)

Este projeto apresenta um **MVP de análise exploratória de fundos de investimento**, com foco em boas práticas de análise de dados, visualização e comunicação clara dos resultados.  
O objetivo é oferecer uma visão didática e acessível sobre métricas de risco e retorno, utilizando Python e ferramentas amplamente adotadas no ecossistema de Data Science.

---

## 🎯 Objetivos do Projeto

- Explorar métricas de risco e retorno de fundos de investimento.  
- Identificar padrões, distribuições e relações entre variáveis.  
- Aplicar boas práticas de análise de dados e visualização.  
- Criar um notebook claro, organizado e didático para avaliação acadêmica.  

---

## 📁 Estrutura do Repositório

```
mvp-fundos-investimento-analise-de-dados-e-boas-praticas/
│
├── data/                         # Arquivos de dados utilizados na análise
│
├── MVP_Fundos_Investimento_...   # Notebook principal do projeto
│
└── README.md                     # Este arquivo
```

---

## 🚀 Como Executar o Notebook

Você pode executar o notebook de duas formas:

### **1. Diretamente no Google Colab (recomendado)**
Clique no botão no topo deste README:

**Open in Colab →** executa tudo sem necessidade de instalação local.

### **2. Localmente na sua máquina**
Requer:

- Python 3.10+  
- Bibliotecas: `pandas`, `numpy`, `matplotlib`, `seaborn`


---

## 📊 Tecnologias Utilizadas

- **Python**  
- **Pandas**  
- **NumPy**  
- **Matplotlib**  
- **Seaborn**  
- **Google Colab**  

---

## 🧩 Hipóteses Avaliadas

Durante a análise exploratória, três hipóteses principais foram levantadas para orientar a investigação dos dados:

1. **Fundos com maior risco (SD) tendem a apresentar maior retorno.**  
2. **O Sharpe Ratio varia significativamente entre categorias de fundos.**  
3. **Fundos com bom desempenho no curto prazo (1 ano) também tendem a performar bem no médio e longo prazo.**

Essas hipóteses serviram como guia para estruturar as visualizações e análises estatísticas apresentadas no notebook.

---

## 🔍 Principais Insights

A análise trouxe alguns achados relevantes:

- A distribuição do risco (desvio‑padrão) é **assimétrica**, com presença de outliers que representam fundos extremamente voláteis.  
- O Sharpe Ratio apresenta **grande variação entre categorias**, reforçando que risco e retorno não se distribuem de forma homogênea no mercado.  
- As correlações entre retornos de 1, 3 e 5 anos mostram **padrões consistentes**, sugerindo que fundos com bom desempenho recente tendem a manter desempenho positivo no médio prazo.  
- O Pairplot evidenciou **relações lineares moderadas** entre algumas métricas, além de destacar clusters visuais que podem indicar perfis distintos de fundos.  
- A análise visual por categoria, com tratamento de outliers apenas para fins de leitura, permitiu comparar grupos de forma mais clara sem alterar os dados originais.

Esses insights ajudam a construir uma visão mais estruturada sobre o comportamento dos fundos e reforçam a importância de combinar múltiplas métricas para avaliar risco e retorno.

---

## 🔮 Próximos Passos

Este MVP cumpre o objetivo de apresentar uma análise clara e didática sobre métricas de risco e retorno de fundos de investimento.  
Caso o projeto seja expandido futuramente, alguns caminhos naturais incluem:

- inclusão de novas métricas (drawdown, tracking error, information ratio)  
- comparação entre diferentes benchmarks  
- análise temporal da evolução dos fundos  
- criação de dashboards interativos (Streamlit ou Power BI)  
- aplicação de modelos de clusterização para segmentar fundos por perfil de risco  

Essas extensões permitiriam aprofundar a análise e transformar o MVP em um estudo mais robusto e completo.

---

## 🙌 Agradecimentos

Obrigado por dedicar tempo para revisar este projeto.  
Feedbacks, sugestões e melhorias são sempre bem-vindos.

---

## 👤 Autor

**Paulo Ricardo**  
Projeto desenvolvido como parte de um MVP acadêmico de análise de dados.
