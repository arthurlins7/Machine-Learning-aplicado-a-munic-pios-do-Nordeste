# 📊 APLICAÇÃO DE TÉCNICAS DE MACHINE LEARNING NA IDENTIFICAÇÃO DE MUNICÍPIOS DO NORDESTE BRASILEIRO COM MAIOR POTENCIAL PARA ATRAÇÃO DE INVESTIMENTOS A PARTIR DE DADOS SOCIOECONÔMICOS

> [cite_start]**Trabalho de Conclusão de Curso** apresentado à faculdade **CESAR School** como requisito para a graduação em Ciência da Computação[cite: 5, 15].

---

## 📝 Resumo
[cite_start]Este trabalho investiga a aplicação de técnicas de **Machine Learning (ML)** para identificar o potencial de atração de investimentos nos municípios do Nordeste brasileiro[cite: 8]. [cite_start]Utilizando uma base de dados socioeconômicos e fiscais públicos (IBGE, SICONFI) do período de 2018 a 2021, o objetivo foi superar limitações de modelos econométricos tradicionais na captura de dinâmicas regionais complexas[cite: 8].

---

## 🚀 Modelagem e Algoritmos
[cite_start]O estudo comparou modelos lineares com algoritmos de *ensemble* baseados em árvores[cite: 8, 40]:

### 🔹 Abordagem de Regressão (Previsão do PIB per capita)
* [cite_start]`OLS (Regressão Linear Múltipla)`: Utilizado como baseline estatístico[cite: 8, 211].
* [cite_start]`Random Forest Regressor`: Modelo baseado em árvores (bagging)[cite: 110, 231].
* [cite_start]`XGBoost Regressor`: Modelo de melhor desempenho baseado em boosting[cite: 110, 241].

### 🔹 Abordagem de Classificação (Faixas de Oportunidade)
* [cite_start]Categorização em municípios de **"Alta Oportunidade"** (acima do quartil P75) e **"Baixa Oportunidade"**[cite: 311].
* [cite_start]Modelos utilizados: `Logistic Regression`, `Random Forest Classifier` e `XGBoost Classifier`[cite: 312, 313, 314, 315].

---

## 🔍 Metodologia e Variáveis
[cite_start]A pesquisa possui natureza aplicada e abordagem quantitativa[cite: 92, 93].

* [cite_start]**Fontes de Dados**: IBGE (PIB, População), Tesouro Nacional (SICONFI/CAPAG) e RAIS/CAGED (Emprego formal)[cite: 101, 102, 103, 104].
* **Engenharia de Atributos**:
    * [cite_start]**Normalização**: Criação de indicadores como `receita_corrente_pc`, `taxa_emprego_formal` e `capex_share`[cite: 123, 130, 131, 132].
    * [cite_start]**Tratamento de Assimetria**: Aplicação de transformação logarítmica ($log1p$) no PIB per capita[cite: 135].
    * [cite_start]**Imputação**: Uso de `Random Forest Classifier` para estimar valores faltantes da nota CAPAG[cite: 105].

---

## 📈 Resultados de Performance
[cite_start]O modelo **XGBoost** demonstrou superioridade em todas as métricas de teste para a região Nordeste[cite: 10, 272].

### Comparativo de Regressão
| Modelo | $R^{2}$ | RMSE | MAE | MAPE (%) |
| :--- | :---: | :---: | :---: | :---: |
| **XGBoost** | **0.882** | **0.158** | **0.117** | **4.61%** |
| Random Forest | 0.862 | 0.171 | 0.127 | 4.98% |
| Linear Regression | 0.761 | 0.225 | 0.157 | 6.10% |

> [Fonte: cite 268]

---

## 🏆 Ranking de Potencial (Top 5 - 2021)
[cite_start]Municípios identificados com os fundamentos econômicos mais sólidos segundo o modelo previsto[cite: 297, 298]:

1.  [cite_start]**Godofredo Viana (MA)** [cite: 298]
2.  [cite_start]**Santo Antônio dos Lopes (MA)** [cite: 298]
3.  [cite_start]**São Bento do Norte (RN)** [cite: 298]
4.  [cite_start]**Formosa do Rio Preto (BA)** [cite: 298]
5.  [cite_start]**São Gonçalo do Amarante (CE)** [cite: 298]

---

## 📌 Conclusões
* [cite_start]**Determinantes**: A receita corrente per capita, taxa de emprego formal e estrutura industrial são os fatores mais críticos para o potencial econômico[cite: 11, 357].
* [cite_start]**Interpretabilidade**: O uso de ML permitiu resolver paradoxos estruturais do OLS, como a relação entre investimento público e riqueza[cite: 10, 262].
* [cite_start]**Impacto**: Oferece uma ferramenta robusta para investidores privados e gestores públicos na identificação de polos de desenvolvimento fora das capitais[cite: 13, 44].

---

[cite_start]**Autor:** Arthur Lins da Gama [cite: 5]
[cite_start]**Orientador:** Guilherme Fernando Cavalcanti Pereira [cite: 6]
[cite_start]**Instituição:** CESAR School, 2025 [cite: 15]
