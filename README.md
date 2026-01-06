# 🛒 Dashboard de Vendas - Supermercado Regional

Projeto de Business Intelligence focado na análise de performance de vendas de três filiais de supermercado, utilizando tratamento de dados no Google Sheets e visualização no Looker Studio.

## 📊 O Resultado Final
> **[Clique aqui para acessar o Dashboard Interativo](https://lookerstudio.google.com/reporting/404af525-7203-4c1d-807a-6381ce5ba1b6)**

![Preview do Dashboard]([print_dashboard_vendas_supermercado.png](https://github.com/larissa-vitoria/analise-vendas-supermercado/blob/a30347cf43ad4eac334c34f71bf82053170b4bfd/assets/print_dashboard_vendas_supermercado.jpg))

## 🛠️ Tecnologias Utilizadas
* **Google Sheets:** Limpeza, transformação e normalização dos dados.
* **Looker Studio:** Modelagem de dados e visualização interativa.

## ⚙️ O Processo de ETL (Extração, Transformação e Carga)

Os dados originais ("Supermarket Sales - Kaggle") continham inconsistências de formatação regional e idioma. O tratamento foi realizado manualmente para garantir a integridade linha a linha:

1.  **Tradução e Localização:** * Adaptação do cenário para o contexto brasileiro (Cidades: Yangon → Florianópolis, etc.).
    * Tradução de categorias de produtos e tipos de clientes.
2.  **Limpeza de Dados:**
    * **Correção de Datas:** Conversão de formatos mistos (americano/texto) para o padrão ISO (DD/MM/AAAA) através de ajustes de localidade na planilha.
    * **Padronização Numérica:** Ajuste de separadores decimais (ponto para vírgula) para leitura correta no Looker Studio.
    * **Remoção de Redundâncias:** Exclusão da coluna "Branch" (redundante com Cidade) e unificação de dados de margem bruta.
3.  **Visualização:**
    * Criação de campos calculados para extração de hora e dia da semana.
    * Cálculo real do Ticket Médio (Média).

## 📈 Principais Insights
* O **Ticket Médio** real é de R$ 323,00.
* O **Horário de Pico** ocorre consistentemente às 19h, indicando necessidade de reforço operacional.
* A categoria **Casa e estilo** lidera o faturamento na filial Florianópolis, enquanto **Acessórios eletrônicos** lideram o faturamento geral.

---
*Este projeto faz parte do meu portfólio de Análise de Dados.*
