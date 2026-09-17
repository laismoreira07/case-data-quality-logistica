# 3. Diagnóstico de qualidade dos dados

## Matriz de inconsistências

| Categoria | Exemplo observado | Risco | Controle proposto |
|---|---|---|---|
| Lote | Lotes físicos misturados ou registro genérico | Perda de rastreabilidade | Validação obrigatória e segregação |
| Validade | Data ausente ou divergente | Seleção incorreta e risco regulatório | Máscara, regra e conferência FEFO |
| Unidade de medida | Embalagem física diferente da unidade cadastrada | Saldo e separação incorretos | Tabela de conversão e revisão cadastral |
| Fornecedor | Duplicidade ou associação inconsistente | Relatórios e compras distorcidos | Identificador único e deduplicação |
| Posição | Item sem endereço confiável | Tempo de procura e inventário impreciso | Endereçamento obrigatório e auditoria |
| Quantidade | Diferença entre contagem e saldo | Ruptura ou excesso aparente | Reconciliação e ajuste controlado |
| Integração | Informações diferentes entre as fontes | Decisão baseada em dado incorreto | Regra de precedência e monitoramento |
| IA no fluxo de coleta | Identificação divergente da evidência física | Propagação de erro na validação | Confirmação humana e registro da falha |

## Dimensões avaliadas

### Completude

Verificação da presença dos atributos mínimos necessários para identificar, armazenar e movimentar o item.

### Consistência

Comparação do mesmo atributo entre Portal de Origem, Delage RX, SIGMA e inventário físico.

### Unicidade

Identificação de registros duplicados ou entidades representadas com mais de uma nomenclatura.

### Validade

Análise de formato e aderência às regras estabelecidas para datas, lotes, unidades e estados do processo.

### Acurácia

Verificação da correspondência entre o valor registrado e a evidência observada.

### Rastreabilidade

Avaliação da possibilidade de reconstruir a origem do dado, as correções realizadas e a movimentação do item.

## Causas agrupadas

As divergências foram organizadas em quatro famílias para evitar que sintomas diferentes recebessem a mesma ação corretiva:

- **Cadastro:** atributo inexistente, incorreto, duplicado ou desatualizado.
- **Processo:** etapa executada fora do padrão ou sem evidência suficiente.
- **Sistema e integração:** regra, disponibilidade ou sincronização inadequada ao fluxo.
- **Operação física:** identificação, segregação, embalagem ou posição divergente.

## Exemplo demonstrativo

O arquivo `data/amostra_inventario_sintetica.csv` permite observar como uma mesma linha pode apresentar mais de uma dimensão comprometida. Todos os seus registros são fictícios e foram elaborados exclusivamente para este portfólio.

