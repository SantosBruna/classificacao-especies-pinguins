# 📊 Projeto: Segmentação de Dados com K-Means (Penguins Dataset)

## 📌 Sobre o Projeto

Projeto desenvolvido no Profissão Cientista de Dados, focado na aplicação de algoritmos de clusterização, especificamente o K-Means, para segmentação de dados biológicos.

Diferente de aplicações tradicionais (como marketing e crédito), este projeto utiliza dados de pinguins para demonstrar a versatilidade do K-Means na identificação de padrões e agrupamentos naturais em diferentes contextos.

O **objetivo principal** é agrupar os indivíduos com base em características físicas e verificar se os clusters encontrados correspondem às espécies reais.

A base utilizada é o dataset Penguins, disponível na biblioteca Seaborn, contendo medições físicas de três espécies de pinguins:

* Adelie
* Chinstrap
* Gentoo
---

## 🎯 Objetivos

* Realizar limpeza e preparação dos dados
* Identificar e tratar valores faltantes
* Selecionar apenas variáveis numéricas para o modelo
* Realizar análise exploratória visual (pairplot)
* Padronizar os dados
* Aplicar o algoritmo K-Means
* Definir número de clusters com base no problema
* Visualizar os clusters e centróides
* Interpretar os agrupamentos gerados

---

## 📁 Estrutura do Projeto

```
├── Profissao Cientista de Dados M30 Pratique.ipynb
└── README.md
```

---

## 🛠️ Tecnologias Utilizadas

* **Python 3.8+**
* **Pandas** - Manipulação e análise de dados
* **NumPy** - Operações numéricas
* **Matplotlib** - Visualização de dados
* **Seaborn** - Visualizações estatísticas avançadas
* **Scikit-learn** - Divisão de dados, pré-processamento, modelagem e métricas de avaliação
* **Jupyter Notebook** - Ambiente de desenvolvimento

---

## 📊 Descrição dos Dados

O dataset contém informações de clientes bancários com as seguintes variáveis:

| Variável | Descrição |
|----------|-----------|
| **species** |Espécie do pinguim |
| **island** | Ilha onde foi observado |
| **bill_length_mm** | Comprimento do bico (mm) |
| **bill_depth_mm** | Profundidade do bico (mm) |
| **flipper_length_mm** | Comprimento da barbatana (mm) |
| **body_mass_g** | Massa corporal (g) |
| **sex** | Sexo |

---

## 📈 Análises Realizadas

### Limpeza e Preparação dos Dados
- Remoção de valores faltantes (missing values)
- Exclusão de variáveis categóricas (não utilizadas no K-Means)
- Manutenção apenas de variáveis numéricas relevantess

### Análise Exploratória (EDA)

Foi utilizado o pairplot para visualizar relações entre variáveis.

📊 Principais Insights:
- bill_depth_mm vs flipper_length_mm → separação clara em 2 grupos
- body_mass_g vs bill_depth_mm → também evidencia 2 clusters bem definidos
- Outras combinações indicam a formação de até 3 grupos, porém com separação menos nítida

💡 Indício inicial de que existem 3 clusters, coerente com o número de espécies.

### Padronização dos Dados
- Aplicação de StandardScaler
- Necessário para garantir que todas as variáveis tenham a mesma escala
- Evita que variáveis com valores maiores dominem o modelo

### Aplicação do K-Means
- Algoritmo utilizado: K-Means
- Número de clusters definido: k = 3
- Justificativa: quantidade de espécies no dataset

### Visualização dos Clusters
Foram construídos gráficos de dispersão com:
- Pontos representando os dados
- Centróides indicando o centro de cada cluster
  
Exemplos analisados:
1. bill_length_mm vs bill_depth_mm
2. Outras combinações de variáveis físicas

### Interpretação dos Resultados
- O modelo conseguiu identificar agrupamentos coerentes com as espécies
- Algumas variáveis apresentam melhor separação natural dos grupos
- Nem todos os clusters são perfeitamente separados (o que é esperado em dados reais)
---

🔍 Aplicações de Clusterização
Além deste exemplo, algoritmos de clusterização são amplamente utilizados em:
1. Sistemas de recomendação musical (Spotify, YouTube, Amazon Music)
  → Agrupamento de usuários por preferência musical
2. Streaming de filmes e séries (Netflix, Prime Video, Disney+)
  → Recomendação baseada em padrões de consumo
3. Atendimento ao cliente
  → Agrupamento de reclamações para identificar problemas recorrentes



🔍 Principais Insights
1. Variáveis físicas permitem segmentar naturalmente as espécies
2. Algumas combinações mostram separação mais clara que outras
3. O K-Means consegue capturar padrões mesmo sem informação de rótulo
4. A padronização é essencial para o bom desempenho do modelo
5. Clusterização é altamente versátil e aplicável em diversas áreas
---

## 👩‍💻 Autora

**Bruna S. R. Santos**

* 🔗 LinkedIn: [www.linkedin.com/in/brunasrsantos](https://www.linkedin.com/in/brunasrsantos)
* 📧 Email: brunasrsantos@gmail.com

---

## 📝 Licença

Este projeto está licenciado sob a **MIT License**.
