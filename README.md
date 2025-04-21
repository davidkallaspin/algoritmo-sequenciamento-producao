# Algoritmo de Sequenciamento de Produção

**Descrição**  
Projeto em `Python` para resolver o problema de sequenciamento de ordens de produção, minimizando tempos de setup, atrasos e considerando a priorização de ordens específicas.

## Detalhes
- **Leitura e pré‑processamento de dados**: importa automaticamente planilha Excel com tempos de setup, datas de necessidade e pesos de prioridade.
- **Geração exaustiva de sequências**: cria todas as permutações possíveis de ordens (complexidade `n!`), garantindo análise completa.
- **Cálculo de função de fitness multi‑critério**: combina minimização de tempo de setup, atrasos e priorização de ordens em uma métrica única.
- **Normalização de métricas pelo pior caso**: padroniza valores heterogêneos (tempo, atraso, prioridade) usando o pior cenário como referência.
- **Visualização de resultados**:
  - Gráficos com `matplotlib` e `Altair`, destacando a melhor sequência;
- **Destacamento automático da melhor solução**: identifica e anota a permutação mais eficiente para extração de insights.
- **Configuração flexível de parâmetros**: ajusta pesos relativos, tolerâncias de atraso e thresholds de setup diretamente no notebook ou via linha de comando.

## Estrutura do Projeto
- `Projeto_Seq_Prod.ipynb`: notebook principal com importação de dados, cálculo de fitness e visualizações.
- `Projeto_Seq_Prod.html`: exportação estática do notebook para visualização offline.
- `production_df.xlsx`: planilha de entrada com tempos de setup, prazos e prioridades.

## Instalação
1. **Clone** este repositório:  
   ```bash
   git clone git@github.com:davidkallaspin/algoritmo-sequenciamento-producao.git
   ```
2. **Crie e ative** um ambiente virtual (macOS/Linux):  
   ```bash
   python3 -m venv venv
   source venv/bin/activate
   ```
3. **Instale** as dependências:  
   ```bash
   pip install -r requirements.txt
   ```

## Uso
- **Notebook**: execute  
  ```bash
  jupyter notebook Projeto_Seq_Prod.ipynb
  ```
- **Visualização estática**: abra `Projeto_Seq_Prod.html` no navegador para ver o relatório gerado.


## Próximos Passos
- Implementar meta‑heurísticas (Simulated Annealing, algoritmos genéticos) para escalabilidade em cenários de produção.  

---

*© David Kallás Pinto*
