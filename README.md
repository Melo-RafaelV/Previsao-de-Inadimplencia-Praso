# Previsão de Inadimplência no Varejo

## Sobre o Projeto
Este projeto de Machine Learning tem como objetivo desenvolver modelos preditivos para avaliar o risco de inadimplência de pequenos varejistas na compra de mercadorias. 

O problema de negócio central gira em torno do ciclo de caixa. Ao conceder prazo para pagamento, fornecedores assumem o risco do não recebimento, o que pode gerar prejuízos. Para mitigar esse risco de forma ágil e sem burocracia, este projeto propõe a criação de escores de risco baseados em dados públicos, dados de birôs de crédito e no próprio histórico comportamental de compras.

O projeto é dividido no desenvolvimento de duas abordagens complementares:
* **Modelo de Aplicação (Novos Clientes):** Estima a probabilidade de um cliente recém-cadastrado ficar inadimplente utilizando apenas informações prévias ao cadastro (ex: situação do CNPJ, consultas de crédito, avaliações em plataformas externas).
* **Modelo Comportamental (Clientes Recorrentes):** Estima a probabilidade de um cliente ativo ficar inadimplente, integrando seu histórico de pedidos (valor das compras, frequência e histórico de dias de atraso).

---

## Metodologia e Etapas
1. **Análise e Pré-processamento de Dados:** Limpeza de dados, tratamento de valores faltantes, remoção de duplicatas, tratamento de outliers e desbalanceamento de classes, além da normalização de variáveis.
2. **Engenharia de Features:** Criação e extração de novas variáveis estratégicas a partir de informações como código CNAE, agrupamento geográfico, e agregação de histórico comportamental (valores médios/máximos de compras e proporção de atrasos).
3. **Modelagem Preditiva:** Treinamento, tunagem de hiperparâmetros e comparação de 3 algoritmos de Machine Learning distintos adequados para classificação.
4. **Avaliação de Resultados:** Análise profunda dos modelos utilizando métricas como **ROC-AUC** (métrica principal de ordenação do risco), Acurácia, Precisão, Recall, F1-Score e tempo de inferência.

---

## Como Rodar o Projeto

### Passo a Passo

- **1. Clone o repositório**
- **2. Baixe os datasets disponibilizados no classroom da disciplina**
- **3. Coloque os datasets na pasta do projeto**
- **4. Rode o notebook**
