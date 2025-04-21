# Algoritmo de Sequenciamento de Produção

**Descrição**  
Projeto em Python para resolver o problema de sequenciamento de ordens de produção, minimizando tempos de setup, atrasos e priorização de pedidos.

## Funcionalidades
- **Leitura e pré‑processamento de dados**: importa automaticamente planilha Excel com tempos de setup, datas de necessidade e pesos de prioridade.
- **Geração exaustiva de sequências**: cria todas as permutações possíveis de ordens (complexidade `n!`), garantindo análise completa.
- **Cálculo de função de fitness multi‑critério**: combina minimização de tempo de setup, atrasos e priorização de ordens em uma métrica única.
- **Normalização de métricas pelo pior caso**: padroniza valores heterogêneos (tempo, atraso, prioridade) usando o pior cenário como referência.
- **Visualização de resultados**:
  - Gráficos estáticos com `matplotlib`, destacando a melhor sequência;
  - Dashboards interativos com `Altair`, permitindo explorar diferentes combinações de pesos.
- **Destacamento automático da melhor solução**: identifica e anota a permutação mais eficiente para fácil extração de insights.
- **Configuração flexível de parâmetros**: ajusta pesos relativos, tolerâncias de atraso e thresholds de setup diretamente no notebook ou via linha de comando.
- **Exportação de relatórios**: gera CSVs com as top‑k melhores sequências e métricas de desempenho.

## Estrutura do Projeto
- `sequenciamento.ipynb`: notebook principal com importação de dados, cálculo de fitness e visualizações.
- `utils.py`: funções auxiliares para leitura de dados, geração de permutações e cálculo de métricas.
- `production_df.xlsx`: planilha de entrada com tempos de setup, prazos e prioridades.
- `.gitignore`: padrões de arquivos ignorados pelo Git.

## Instalação
1. Clone este repositório:
   ```bash
   git clone git@github.com:davidkallaspin/algoritmo-sequenciamento-producao.git
