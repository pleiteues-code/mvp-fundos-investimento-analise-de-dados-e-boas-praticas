# 📊 MVP – Análise de Fundos de Investimento

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/pleiteues-code/mvp-fundos-investimento-analise-de-dados-e-boas-praticas/blob/main/MVP_Fundos_Investimento_Paulo_Ricardo_Marques_Leite.ipynb)

Este repositório contém o MVP desenvolvido para a disciplina **Análise de Dados e Boas Práticas**, com foco na avaliação de fundos de investimento utilizando métricas de risco, retorno e eficiência.

---

## 👤 Autor

**Nome:** Paulo Ricardo Marques Leite  
**Matrícula:** 4052025002553  

---

## 📁 Estrutura do Repositório

| Caminho | Descrição |
|--------|-----------|
| `data/comprehensive_mutual_funds_data.csv` | Dataset utilizado no projeto |
| `MVP_Fundos_Investimento_Paulo_Ricardo_Marques_Leite.ipynb` | Notebook completo |
| `README.md` | Documentação do projeto |

---

## 📝 Descrição do Projeto

O objetivo deste MVP é analisar um conjunto real de fundos de investimento, avaliando:

- **Risco:** desvio-padrão  
- **Retorno:** janelas de 1, 3 e 5 anos  
- **Eficiência:** Sharpe, Sortino, Alpha e Beta  

A análise busca responder perguntas práticas sobre o comportamento dos fundos e validar hipóteses relacionadas ao equilíbrio entre risco e retorno.

---

## 🔍 Hipóteses Avaliadas

1. Fundos com maior **Sharpe Ratio** tendem a apresentar retornos mais altos.  
2. Fundos mais arriscados (maior desvio-padrão) **não necessariamente** entregam melhor retorno.  
3. Categorias diferentes de fundos apresentam padrões distintos de risco e retorno.

---

## 🧪 Metodologia

O notebook inclui:

- Carregamento e inspeção inicial do dataset  
- Limpeza e preparação dos dados
  - tratamento de valores ausentes
  - conversão de colunas numéricas
  - padronização das categorias (correção de variações como “Custom Oriented”, “Solution oriented”, “Non-Oriented”) 
- Visualizações exploratórias  
- Matriz de correlação  
- Teste das hipóteses  
- Conclusões finais  

---
## 📌 Função de visualização
Para evitar repetição de código e garantir consistência visual, foi criada a função:

def plot_box(df, x, y, order, title, ylabel, ylim=None):
    plt.figure(figsize=(10,5))
    
    sns.boxplot(
        x=x,
        y=y,
        data=df,
        order=order,
        hue=x,
        palette='viridis',
        legend=False,
        linewidth=1.5
    )
    
    plt.xticks(rotation=45)
    plt.title(title)
    plt.xlabel("Categoria")
    plt.ylabel(ylabel)
    plt.grid(axis='y', linestyle='--', alpha=0.3)
    
    if ylim:
        plt.ylim(0, ylim)
    
    plt.tight_layout()
    plt.show()
    
    Essa função padroniza:
- paleta
- grid
- espessura das linhas
- layout
- ordem das categorias
E permite ajustes futuros em um único ponto.

---
## 🛠 Tecnologias Utilizadas

- Python  
- Pandas  
- Seaborn  
- Matplotlib  
- Google Colab  

---

## 🔗 Links Importantes

**Notebook no Google Colab (esse é o original em meu Drive, mas o botão no início desse documento faz referência à cópia salva aqui):**  
https://colab.research.google.com/drive/1oDmkxqFGegxdV9t8aoXHfmnIIFP8J_hj#scrollTo=DBKjBRbGHmTq

**Dataset (RAW):**  
https://raw.githubusercontent.com/pleiteues-code/mvp-fundos-investimento-analise-de-dados-e-boas-praticas/main/data/comprehensive_mutual_funds_data.csv

**Fonte do Dataset (Kaggle):**  
https://www.kaggle.com/datasets/iamsouravbanerjee/mutual-funds-india

---

## 📈 Resultado Final

O MVP demonstra que métricas de risco e retorno podem ser utilizadas para:

- Comparar fundos de forma objetiva  
- Identificar eficiência ajustada ao risco  
- Entender diferenças entre categorias de fundos  

---
## 🧪 Resultados das Hipóteses

• 	Hipótese 1: parcialmente confirmada — Sharpe se correlaciona moderadamente com retornos de 3 anos.
• 	Hipótese 2: refutada — maior risco não implica maior eficiência.
• 	Hipótese 3: confirmada — categorias apresentam padrões distintos de Sharpe e SD.


O MVP demonstra que métricas de risco e retorno podem ser utilizadas para:

- Comparar fundos de forma objetiva  
- Identificar eficiência ajustada ao risco  
- Entender diferenças entre categorias de fundos  

---
## 📬 Contato

Caso deseje mais informações ou tenha dúvidas, entre em contato:  
📧 **pleiteues@gmail.com**

