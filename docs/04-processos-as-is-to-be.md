# 4. Processos AS-IS e TO-BE

## AS-IS consolidado

```mermaid
flowchart TD
    A[Solicitação no Portal de Origem] --> B[Registro e tratamento nos sistemas]
    B --> C[Recebimento ou separação física]
    C --> D[Leitura e validação operacional]
    D --> E{Dados aderentes?}
    E -- Sim --> F[Movimentação concluída]
    E -- Não --> G[Ajuste manual ou tratamento de exceção]
    G --> H[Registro nem sempre padronizado]
    H --> I[Possível reincidência]
```

### Fragilidades principais

- validações distribuídas entre diferentes pessoas e fontes;
- dependência de conhecimento tácito;
- tratamento de exceções sem classificação única;
- risco de ajuste do saldo sem eliminação da causa;
- inconsistências descobertas tardiamente, durante separação ou inventário;
- resposta da IA necessitando conferência quando divergente da evidência física.

## TO-BE proposto

```mermaid
flowchart TD
    A[Solicitação estruturada] --> B[Validações de cadastro e regra]
    B --> C{Registro válido?}
    C -- Não --> D[Fila de saneamento]
    D --> B
    C -- Sim --> E[Execução operacional]
    E --> F[Conferência física e sistêmica]
    F --> G{Divergência?}
    G -- Sim --> H[Classificar causa e tratar]
    H --> I[Revalidar e registrar evidência]
    G -- Não --> J[Concluir movimentação]
    I --> J
    J --> K[Indicadores e melhoria contínua]
```

## Princípios do desenho futuro

1. **Prevenir antes de corrigir:** validar atributos críticos na entrada.
2. **Separar sintoma de causa:** não tratar toda divergência como ajuste de estoque.
3. **Registrar exceções:** manter categoria, responsável, evidência e decisão.
4. **Revalidar:** confirmar o resultado após qualquer correção.
5. **Medir reincidência:** observar se a mesma causa volta a ocorrer.
6. **Manter supervisão humana:** revisar resultados de IA em situações de baixa confiança ou conflito com evidências.

## Responsabilidades sugeridas

| Papel | Responsabilidade |
|---|---|
| Operação | Registrar evidência e executar a conferência física |
| Qualidade ou governança | Validar regra, causa e necessidade de saneamento |
| TI e sistemas | Tratar parametrização, integração e indisponibilidade |
| Dono do processo | Priorizar riscos e aprovar mudanças de procedimento |
| Gestão | Acompanhar indicadores, reincidências e plano de ação |

