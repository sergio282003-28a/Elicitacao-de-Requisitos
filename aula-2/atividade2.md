Atividade: Making History

Disciplina: Elicitação de Requisitos
Contexto: Aplicativo de delivery de comida

História 1 — Acompanhar o pedido

História de usuário: Como cliente, quero consultar o status do meu pedido após a compra para saber em que etapa ele está até a entrega.

Critérios de aceitação

1. Dado que concluí uma compra, quando abro os detalhes do pedido, então vejo seu status atual.

2. Dado que o restaurante ou o entregador atualizou a etapa do pedido, quando consulto os detalhes novamente, então vejo o novo status e o horário dessa atualização.

3. Dado que o pedido foi entregue, quando consulto seu histórico, então vejo o status “Entregue” e o horário da entrega.

História 2 — Indicar item indisponível

História de usuário: Como responsável pelo restaurante, quero marcar um item do cardápio como indisponível para impedir que clientes façam novos pedidos desse item enquanto ele estiver em falta.

Critérios de aceitação

1. Dado que um item está disponível no cardápio, quando o marco como indisponível no painel do restaurante, então ele deixa de poder ser adicionado a novos pedidos.

2. Dado que um cliente colocou o item no carrinho antes de ele ficar indisponível, quando tenta concluir a compra, então o aplicativo informa a indisponibilidade e impede a finalização com esse item.

3. Dado que o item está marcado como indisponível, quando o restaurante o marca novamente como disponível, então os clientes podem adicioná-lo a novos pedidos.

História 3 — Reportar problema na entrega

História de usuário: Como entregador, quero registrar um problema em uma entrega em andamento para que a equipe de suporte possa agir com base no ocorrido.

Critérios de aceitação

1. Dado que tenho uma entrega em andamento, quando abro os detalhes dessa entrega, então encontro a opção de reportar um problema.

2. Dado que abri a opção de reportar um problema, quando seleciono o motivo e confirmo o envio, então o aplicativo registra o relato vinculado ao pedido e confirma que ele foi enviado ao suporte.

3. Dado que não selecionei um motivo, quando tento enviar o relato, então o aplicativo solicita essa informação e não registra um relato incompleto.


Priorização com MoSCoW

Ordem História Prioridade Justificativa

1.

Indicar item indisponível

Must have

Evita que o cliente compre algo que o restaurante não consegue entregar.

2.

Reportar problema na entrega

Should have

Ajuda o suporte a agir durante uma entrega com problema; o serviço ainda pode operar inicialmente com atendimento por outro canal.

3.

Acompanhar o pedido

Should have

Dá visibilidade ao cliente e reduz a incerteza após a compra, mas o pedido pode ser realizado e entregue antes dessa melhoria.

 Nenhuma das três demandas foi classificada como Could have ou Won't have, pois todas têm valor para o funcionamento do serviço e estão consideradas para desenvolvimento. A ordem entre os dois itens Should have considera a urgência de lidar com problemas durante uma entrega. Essa prioridade pode ser revista após conversar com clientes, restaurantes, entregadores e suporte.
