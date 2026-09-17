# 6. Governança, riscos e aprendizados

## Controles de governança

- dicionário dos atributos críticos;
- definição de fonte e responsável por cada dado;
- critérios de aceite e rejeição;
- histórico de correções e evidências;
- fluxo formal para exceções;
- revisão periódica de cadastros;
- monitoramento de reincidências;
- separação entre ambiente de homologação e produção;
- comunicação de indisponibilidades e contingências.

## Riscos tratados

| Risco | Impacto possível | Resposta recomendada |
|---|---|---|
| Divergência físico × sistema | Ruptura, excesso aparente ou decisão incorreta | Reconciliação periódica e causa raiz |
| Lote ou validade inconsistente | Perda de rastreabilidade | Validação obrigatória e evidência |
| Unidade de medida inadequada | Erro de quantidade e separação | Tabela de conversão governada |
| Posição inexistente | Aumento do tempo de procura | Endereçamento e auditoria |
| Duplicidade cadastral | Fragmentação do histórico | Regras de unicidade e deduplicação |
| Falha no apoio de IA | Aceite de identificação incorreta | Confirmação humana e telemetria funcional |
| Indisponibilidade sistêmica | Operação paralela sem sincronização | Contingência e reconciliação posterior |

## Aprendizados

### Inventário é também um projeto de dados

A contagem física revela sintomas, mas a confiabilidade depende do tratamento das regras, cadastros, integrações e responsabilidades que produziram as divergências.

### O fluxo real precisa ser observado

Procedimentos documentados não substituem a observação em campo. O AS-IS deve representar decisões, exceções e limitações efetivamente encontradas.

### Tecnologia não elimina a necessidade de governança

WMS, integrações e IA apoiam a operação, mas precisam de dados consistentes, critérios de validação e acompanhamento humano.

### Resultado deve ser demonstrável

Cada recomendação precisa estar vinculada a uma evidência, um risco e um resultado esperado. Percentuais de melhoria somente devem ser divulgados quando houver linha de base e medição posterior comparável.

## Competências demonstradas

- análise de negócio e processos;
- qualidade e governança de dados;
- integração entre sistemas e operação física;
- gestão de stakeholders;
- análise de causa raiz;
- liderança funcional em campo;
- comunicação executiva;
- melhoria contínua e desenho de controles.

