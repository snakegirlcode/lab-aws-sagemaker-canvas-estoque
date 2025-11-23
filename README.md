# 🧠 Previsão de Estoque Inteligente com Amazon SageMaker Canvas

Este repositório contém o desenvolvimento do Lab da DIO, onde construí um modelo de Machine Learning **no-code** usando o **Amazon SageMaker Canvas** para prever níveis de estoque de forma automática.

---

## 🚀 Objetivo do Projeto
Criar um modelo de previsão de estoque sem escrever código, utilizando o SageMaker Canvas, e documentar o processo completo para fins de portfólio.

---

## 📂 Dataset Utilizado

### Exemplo de dataset fictício utilizado

| data       | produto         | categoria | vendas_7dias | estoque_atual | estoque_final |
|------------|-----------------|-----------|--------------|----------------|----------------|
| 2024-02-01 | Arroz Tipo 1    | Alimentos | 42           | 120            | 78             |
| 2024-02-01 | Sabonete Neutro | Higiene   | 15           | 60             | 45             |
| 2024-02-01 | Refrigerante 2L | Bebidas   | 33           | 80             | 47             |

Dataset utilizado: **estoque_supermercado_2024.csv**

---

## 🛠️ Passo a Passo do Desenvolvimento

Para realizar o projeto, iniciei fazendo o upload do dataset fictício `estoque_supermercado_2024.csv` dentro do Amazon SageMaker Canvas. Após o envio, conferi o esquema das colunas para garantir que todas as informações — como vendas dos últimos dias, categoria do produto e estoques — haviam sido reconhecidas corretamente.

Em seguida, criei um novo modelo dentro do Canvas e selecionei a coluna **`estoque_final`** como variável alvo, já que o objetivo era prever o estoque estimado após determinado período. As demais colunas foram automaticamente consideradas como variáveis de entrada, incluindo dados como `vendas_7dias`, `categoria_produto` e `estoque_atual`.

Depois configurei o treinamento e optei pela construção padrão (Standard Build), permitindo que o Canvas realizasse uma análise mais profunda das relações entre as variáveis. Ao final do treinamento, examinei as métricas fornecidas, principalmente a acurácia do modelo e a lista de features mais relevantes para a previsão.

Com o modelo validado, utilizei a ferramenta de previsão do SageMaker Canvas para gerar resultados com base no próprio dataset, simulando como o estoque se comportaria em diferentes cenários. Em seguida, exportei os dados gerados para análise.

## 📊 Resultados Obtidos
- O modelo apresentou boa precisão nas previsões semanais
- Variáveis relacionadas a vendas recentes tiveram maior impacto
- Possibilita reduzir perdas e evitar rupturas em períodos de alta demanda

---

## 🧩 Tecnologias Utilizadas
- **Amazon SageMaker Canvas**
- **Machine Learning no-code**
- **AWS S3** (para armazenamento)
- **GitHub**

---

## 🧑‍💻 Autora
Thaís de Sousa Campos

