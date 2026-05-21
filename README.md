# 🏡 Previsão de preços de imóveis com Machine Learning
O objetivo principal desse projeto foi desenvolver e avaliar um modelo de Machine Learning capaz de prever o preço de venda de casas com base em suas características físicas.

---

## 📌 Contexto
No mercado imobiliário, precificar um imóvel de forma errada pode significar prejuízo para o vendedor ou meses com o imóvel parado no catálogo. Este projeto simula uma solução para empresas do setor, automatizando o cálculo de estimativa de preço com base em dados históricos para dar mais segurança e agilidade aos corretores.

## 📊 Conjunto de dados
Os dados utilizados neste projeto contam com informações estruturadas sobre imóveis, incluindo as seguintes variáveis principais:
* `area_m2`: Área útil ou construída do imóvel.
* `quartos`: Quantidade de dormitórios.
* `vagas_garagem`: Vagas de estacionamento disponíveis.
* `preco_venda`: O preço final de venda.

## 🛠️ Tecnologias e ferramentas utilizadas
* **Linguagem:** Python
* **Manipulação de dados:** Pandas e NumPy
* **Visualização de dados:** Matplotlib e Seaborn
* **Machine Learning:** Scikit-Learn (algoritmo de regressão linear)

## 🚀 Ciclo de desenvolvimento do projeto
O projeto foi estruturado seguindo as melhores práticas do pipeline de ciência de dados:

1. **Entendimento dos dados:** Leitura da base e identificação das variáveis explicativas e da variável alvo.
2. **Divisão de dados:** Separação estrita da base de dados usando a técnica `train_test_split` (80% para treino do algoritmo e 20% para testes independentes), garantindo que o modelo seja avaliado com dados que ele nunca viu antes.
3. **Treinamento do modelo:** Instanciação e ajuste do algoritmo de regressão linear utilizando os dados de treino.
4. **Previsão e avaliação:** Geração de previsões automáticas para os dados de teste e comparação matemática entre os preços reais e os "chutes" do modelo.

## 📈 Resultados e métricas do modelo
Após rodar o modelo completo, o desempenho foi avaliado através de duas métricas principais:

* **MAE (Erro Médio Absoluto):** [Insira aqui o valor do MAE que apareceu no seu terminal, ex: R$ 15.230,00]
  * O que significa: Em média, as previsões do modelo erram o valor real da casa por esta margem (para mais ou para menos).
* **R² (Score de Precisão):** [Insira aqui o valor do R2 que apareceu no seu terminal, ex: 0.94]
  * O que significa: O modelo consegue explicar [ex: 94%] da variação dos preços das casas usando apenas as características fornecidas.

### 🔍 Amostra prática (Previsão vs. Realidade)
Abaixo está um exemplo de como o modelo se comportou na prática testando imóveis novos:

| Preço Real | Previsão do Modelo | Diferença (R$) |
| :--- | :--- | :--- |
| R$ 550.000,00 | R$ 542.100,00 | R$ 7.900,00 |
| R$ 195.000,00 | R$ 203.400,00 | R$ 8.400,00 |

Obs: Você pode substituir os valores da tabela acima pelos números reais que a sua tabela de comparação gerou na tela

---

## 🧑‍💻 Como Executar este Projeto

1. Clone o repositório para a sua máquina.
2. Abra o arquivo projeto_imoveis.ipynb no seu VS Code ou ambiente Jupyter Notebook.
3. Certifique-se de ter as bibliotecas instaladas (pandas, scikit-learn, matplotlib, seaborn).
4. Execute as células de código sequencialmente.
