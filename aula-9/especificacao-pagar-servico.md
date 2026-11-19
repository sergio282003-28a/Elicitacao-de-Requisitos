# Aula 9 — Especificação de caso de uso

## Sistema e visão do diagrama

**Sistema:** Sistema de Gestão da Oficina de Motos.  
**Atores principais:** Cliente e Atendente.  
**Ator secundário:** Sistema de Pagamentos (serviço externo).  
**Casos de uso:** Solicitar serviço; Consultar andamento; Pagar serviço; Registrar ordem de serviço; Atualizar andamento.

## UC-03 — Pagar serviço

**Ator principal:** Cliente.  
**Ator secundário:** Sistema de Pagamentos.  
**Descrição:** Permite ao cliente pagar uma ordem de serviço concluída e registrar a confirmação do pagamento na oficina.  
**Gatilho:** O cliente seleciona a opção **Pagar serviço** em uma ordem de serviço concluída.

**Pré-condições:**

1. O cliente está identificado no sistema.
2. A ordem de serviço pertence ao cliente, está concluída, tem valor definido e ainda não foi paga.

**Pós-condições:**

- Em caso de sucesso, a ordem de serviço fica marcada como paga, com identificação da transação e comprovante disponível ao cliente.
- Em caso de falha, a ordem de serviço permanece sem pagamento confirmado.

### Fluxo principal

1. O cliente abre a ordem de serviço e seleciona **Pagar serviço**.
2. O sistema exibe o valor devido e os meios de pagamento disponíveis.
3. O cliente escolhe um meio de pagamento e confirma a operação.
4. O sistema envia a solicitação de cobrança ao Sistema de Pagamentos.
5. O Sistema de Pagamentos autoriza a transação e devolve sua identificação.
6. O sistema registra a identificação da transação, marca a ordem de serviço como paga e disponibiliza o comprovante.
7. O sistema apresenta a confirmação ao cliente.

### Fluxo alternativo A1 — Pagamento recusado

**Quando:** No passo 5, o Sistema de Pagamentos responde que a transação foi recusada.

1. O sistema informa a recusa, sem marcar a ordem de serviço como paga.
2. O cliente escolhe outro meio de pagamento ou corrige os dados informados.

**Retorno:** Volta ao passo 3 do fluxo principal para uma nova tentativa. Se o cliente desistir, o caso de uso termina e a ordem continua sem pagamento.

### Exceção E1 — Serviço de pagamentos indisponível

**Quando:** No passo 4 ou 5, não é possível enviar a cobrança ou receber uma resposta do Sistema de Pagamentos.

1. O sistema informa que não foi possível confirmar a operação.
2. O sistema registra a tentativa sem alterar a situação da ordem de serviço para **paga**.
3. O cliente encerra a tentativa.

**Retorno:** O caso de uso é encerrado. Quando o serviço voltar, o cliente pode iniciar novamente pelo passo 1; antes de gerar nova cobrança, o sistema deve verificar se a transação anterior foi confirmada para evitar cobrança duplicada.
