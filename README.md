# 📊 Análise de Desempenho de Lojas (Challenge Data Science)

Projeto de análise exploratória e visualização de dados em **Python** (desenvolvido em **Google Colab**), avaliando o desempenho de quatro lojas (`loja_1`, `loja_2`, `loja_3` e `loja_4`) com base em **9.435 registros** de compras para apoiar uma recomendação estratégica sobre qual loja vender.

## 📌 Sobre o Projeto

O notebook importa os arquivos CSV referentes às quatro lojas, unifica os dados em um único DataFrame (`lojas_unidas`) adicionando a coluna `Loja`, verifica a integridade dos dados (sem valores nulos) e analisa indicadores como faturamento total (`Preço + Frete`), volume de vendas por categoria e por loja, avaliação média dos clientes, produtos de maior e menor valor e frete médio por loja

### ✨ Principais Análises e Resultados

- **Consolidação e qualidade dos dados:** Unificação de 4 bases de dados totalizando **9.435 linhas** e **13 colunas** iniciais (`Produto`, `Categoria do Produto`, `Preço`, `Frete`, `Data da Compra`, `Vendedor`, `Local da compra`, `Avaliação da compra`, `Tipo de pagamento`, `Quantidade de parcelas`, `lat`, `lon` e `Loja`), com **0 valores nulos**
- **Faturamento total (`Preço + Frete`):** A `loja_1` lidera o faturamento total, seguida por `loja_2` e `loja_3`, enquanto a `loja_4` registra o menor faturamento total entre as quatro unidades
- **Vendas por categoria:** `eletronicos` e `eletrodomesticos` concentram os maiores volumes de vendas em valor, seguidos por `moveis`, enquanto categorias como `livros` representam a menor parcela do faturamento
- **Vendas por loja e avaliação:** A `loja_1` apresenta o maior total de vendas em `Preço`, enquanto a `loja_3` e a `loja_2` figuram no topo da média de avaliação das compras (em torno de 4,04 e 4,03, respectivamente, em uma escala de 1 a 5)
- **Produtos mais e menos vendidos (em valor):** Entre os destaques de maior valor acumulado estão *TV Led UHD 4K*, *Celular Plus X42* e *Geladeira*; entre os de menor valor acumulado aparecem *Cubo mágico 8x8*, *Corda de pular* e *Dinossauro Rex*
- **Frete médio por loja:** Comparação da média de `Frete` entre `loja_1`, `loja_2`, `loja_3` e `loja_4` (com média geral de ~33,17 nas transações analisadas)
- **Recomendação estratégica:** Com base nos indicadores avaliados (faturamento, volume de vendas e desempenho por categoria), o relatório aponta a **`loja_4`** como a principal candidata à venda, destacando também a importância de considerar margem de lucro, custos operacionais, potencial de crescimento e localização antes da decisão final

## 🚀 Tecnologias Utilizadas

- **Python 3** (ambiente Google Colab / Jupyter Notebook)
- **Pandas** — Importação de CSVs, concatenação (`pd.concat`), inspeção (`info()`, `isnull()`, `describe()`) e agrupamentos (`groupby()`)
- **Matplotlib** — Criação de gráficos de pizza e barras
- **Seaborn** — Visualizações estatísticas e paletas de cores nos gráficos de barras

## 📂 Estrutura do Projeto

```text
Projeto-Challenge/
└── (notebook .ipynb)   # Importação, unificação, análises, gráficos e relatório final