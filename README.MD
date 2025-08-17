# Challenge Telecom X: análise de evasão de clientes - Parte 2

### **Descrição do Projeto**

Este projeto representa a segunda fase da análise da empresa Telecom X. O objetivo principal aqui é construir e avaliar um **pipeline de Machine Learning** capaz de prever quais clientes têm maior probabilidade de cancelar seus serviços (Churn). A partir de modelos preditivos, foi possível identificar os clientes em risco para que a empresa possa agir com estratégias de retenção mais eficazes, transformando dados em insights de negócio.

### **Tecnologias Utilizadas**

* **Python**: A linguagem de programação principal, utilizada para todo o pipeline.
* **Jupyter Notebook**: O ambiente de desenvolvimento interativo para a análise.
* **Pandas**: Biblioteca essencial para a preparação, limpeza e manipulação dos dados.
* **Scikit-learn**: A principal biblioteca de Machine Learning, utilizada para a criação, treinamento e avaliação dos modelos preditivos.
* **Matplotlib & Seaborn**: Utilizadas para a visualização dos dados e das métricas de avaliação.

### **Análise e Conclusão**

Nesta etapa, dois modelos de classificação foram desenvolvidos e comparados: **Regressão Logística** e **Árvore de Decisão**. Após a avaliação rigorosa de métricas como precisão, recall e F1-score, o modelo de **Regressão Logística** demonstrou o melhor desempenho, com maior capacidade de prever corretamente os clientes que irão cancelar os serviços.

Com base na análise de importância das variáveis deste modelo, foi possível confirmar e aprofundar os insights da primeira fase do projeto. Os principais fatores de risco para a evasão de clientes são:

* **Tempo de contrato (`tenure`)**: Clientes com menos tempo de casa apresentam um risco significativamente maior de Churn.
* **Contrato Mês-a-mês**: A ausência de um contrato de longo prazo é um dos maiores preditores de evasão.
* **Tipo de serviço de internet**: Clientes com serviço de **Fibra Óptica** têm maior propensão a cancelar, o que pode indicar problemas de qualidade ou custo elevado.
* **Custo e método de pagamento**: O `Charges.Total` e o uso de **Cheque Eletrônico** como método de pagamento também foram identificados como fatores de risco.
* **Serviços de Valor Agregado**: A ausência de serviços como Suporte Técnico e Segurança Online aumenta a probabilidade de Churn.

Por essas razões, a empresa deve concentrar seus esforços de retenção nos clientes que se encaixam neste perfil de risco. As estratégias recomendadas incluem o desenvolvimento de programas de fidelização para clientes recém-chegados, o incentivo de contratos de longo prazo e a investigação da qualidade dos serviços que mais geram insatisfação.

### **Próximos Passos**

* Otimização do modelo vencedor (Regressão Logística).
* Testar modelos mais avançados, como Random Forest ou Gradient Boosting.
* Desenvolvimento de um sistema de alerta para identificar clientes em risco em tempo real.