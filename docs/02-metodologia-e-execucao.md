# 2. Metodologia e execução

## Abordagem

O trabalho foi conduzido por ciclos curtos de observação, conferência, comparação e validação. A estratégia evitou tratar o inventário apenas como contagem: cada divergência foi analisada como um possível sintoma de problema cadastral, processual, sistêmico ou operacional.

## Etapas

### 1. Descoberta em campo

- acompanhamento presencial da operação;
- entrevistas com usuários e responsáveis pelos processos;
- observação de entradas, saídas, staging e armazenagem;
- identificação de controles manuais e dependências de conhecimento tácito;
- registro de dúvidas, exceções e hipóteses de causa.

### 2. Mapeamento AS-IS

- representação dos fluxos reais, e não apenas dos procedimentos previstos;
- identificação dos pontos de entrada e transformação dos dados;
- registro das decisões manuais e das exceções;
- associação entre etapa operacional, sistema utilizado e evidência gerada.

### 3. Perfil e classificação dos dados

Os atributos críticos foram agrupados por dimensão:

| Grupo | Exemplos |
|---|---|
| Identificação | SKU, descrição, fabricante e fornecedor |
| Rastreabilidade | lote, validade e histórico de movimentação |
| Quantidade | saldo, embalagem e unidade de medida |
| Localização | endereço, posição e área de armazenagem |
| Integração | origem, status e correspondência entre sistemas |

### 4. Inventário e reconciliação

Para cada ocorrência, buscou-se comparar:

1. o item encontrado fisicamente;
2. o registro correspondente no Delage RX;
3. as informações disponíveis no SIGMA;
4. a solicitação ou referência do Portal de Origem;
5. as evidências complementares coletadas em campo.

### 5. Saneamento e revalidação

- correção de atributos conforme regra validada;
- padronização de formatos e nomenclaturas;
- identificação de duplicidades;
- associação ou revisão de posições;
- revalidação do dado após o tratamento;
- manutenção de evidência para auditoria e acompanhamento.

### 6. Desenho TO-BE

O cenário futuro foi orientado a reduzir a criação de novas inconsistências. As recomendações consideraram validações na entrada, responsabilidades claras, tratamento controlado de exceções, indicadores e ciclos de revisão.

## Uso da IA no fluxo do WMS

O processo utilizava um recurso nativo de IA associado ao fluxo de coleta e validação integrado ao WMS. A atuação no projeto foi funcional: observar resultados, comparar a resposta com as evidências físicas e sistêmicas, registrar falhas, classificar padrões e encaminhar necessidades de ajuste.

Não foram presumidos o algoritmo, o modelo ou a arquitetura interna da solução. O foco foi a qualidade do resultado entregue ao processo e o impacto operacional quando a leitura ou identificação não correspondia à evidência real.

## Critério de encerramento de uma ocorrência

Uma divergência somente poderia ser considerada tratada quando:

- sua causa ou categoria estivesse registrada;
- o valor correto estivesse sustentado por evidência;
- a atualização necessária tivesse sido realizada ou formalmente encaminhada;
- a informação fosse revalidada;
- o histórico permitisse rastrear a decisão.

