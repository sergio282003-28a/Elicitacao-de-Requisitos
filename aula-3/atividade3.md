# Atividade — Requisitos não funcionais

**Disciplina:** Elicitação de Requisitos  
**Contexto:** aplicativo de delivery de comida  
**Referência:** histórias e critérios da atividade da aula 3

Os valores numéricos abaixo são metas propostas para tornar cada requisito testável. Em um projeto real, o Product Owner e a equipe validariam esses limites com os interessados.

## História 1 — Avaliar o pedido após a entrega

> Como cliente, quero avaliar o pedido depois da entrega, para ajudar outros clientes a escolherem melhor.

| ID | Requisito não funcional (RNF) | Característica da ISO/IEC 25010 |
| --- | --- | --- |
| RNF-01 | Após o cliente confirmar uma avaliação, a publicação da nota e do comentário no perfil do restaurante deve ocorrer em até **2 segundos em 95% dos envios**, com até **1.000 envios simultâneos**. | **Eficiência de desempenho** |
| RNF-02 | Em um teste com **20 clientes que ainda não utilizaram a função**, pelo menos **18** devem conseguir localizar a opção de avaliação e publicar nota e comentário em até **60 segundos**, sem ajuda. | **Usabilidade** |
| RNF-03 | Uma avaliação cujo envio foi confirmado deve continuar disponível após reinício do serviço; em **100 testes de reinício após confirmação**, nenhuma avaliação confirmada pode desaparecer. | **Confiabilidade** |

## História 2 — Salvar cartão de pagamento

> Como cliente, quero salvar um cartão de pagamento, para não digitar os dados a cada compra.

| ID | Requisito não funcional (RNF) | Característica da ISO/IEC 25010 |
| --- | --- | --- |
| RNF-04 | O aplicativo deve armazenar e recuperar o cartão por meio de um **token do provedor de pagamento**, sem persistir o número completo do cartão ou seu código de segurança nos bancos de dados do aplicativo. | **Segurança** |
| RNF-05 | A lista de cartões salvos deve aparecer no checkout em até **1,5 segundo em 95% das consultas**, com até **1.000 usuários consultando simultaneamente**. | **Eficiência de desempenho** |
| RNF-06 | A consulta aos cartões salvos deve apresentar **disponibilidade mensal mínima de 99,9%**, medida por verificações automáticas a cada minuto. | **Confiabilidade** |

## História 3 — Consultar resumo de vendas

> Como dono de restaurante, quero ver um resumo diário de vendas, para acompanhar o desempenho do dia.

| ID | Requisito não funcional (RNF) | Característica da ISO/IEC 25010 |
| --- | --- | --- |
| RNF-07 | O painel deve exibir ou recalcular o resumo de um período de até **12 meses** em até **3 segundos em 95% das consultas**, considerando restaurantes com até **10.000 pedidos no período**. | **Eficiência de desempenho** |
| RNF-08 | O resumo de vendas de um restaurante deve ser acessível apenas por contas autenticadas e autorizadas para aquele restaurante; testes de acesso com contas de outros restaurantes devem receber **acesso negado em 100% das tentativas**. | **Segurança** |
| RNF-09 | Em um teste com **20 responsáveis por restaurantes que ainda não utilizaram o painel**, pelo menos **18** devem conseguir identificar o total de pedidos e o faturamento do dia em até **30 segundos**, sem ajuda. | **Usabilidade** |

**Total:** 9 requisitos não funcionais, sendo 3 por história. Cada requisito descreve uma qualidade mensurável da funcionalidade, complementando o comportamento já definido pelos critérios de aceitação.
