# Atividade — Sua vez de elicitar

**Disciplina:** Elicitação de Requisitos  
**Cenário:** empresa que vende por telefone e em encontros presenciais

Os nove requisitos abaixo são **propostas iniciais** para especificar com as fontes indicadas. Como o sistema será criado do zero, não se pressupõe a existência de um sistema legado. Os documentos citados devem ser procurados e conferidos com as pessoas que executam cada processo; se algum não existir, será preciso levantar a regra diretamente com elas.

## Processo 1 — Registrar pedidos (vendedores)

### R01 — Dados do pedido

**Requisito.** O sistema deve permitir que o vendedor registre um pedido com canal da venda (telefone ou presencial), cliente, produtos e quantidades solicitadas.

- **Fonte 1.** Entrevista com vendedores sobre os dados que anotam durante a venda. **Fonte humana, nível operacional, classe de usuário vendedor.**
- **Fonte 2.** Consulta aos formulários ou anotações usados atualmente para registrar vendas. **Fonte não humana, categoria documentação.**

### R02 — Cálculo do total

**Requisito.** O sistema deve calcular o valor total do pedido a partir do preço registrado para cada produto e da quantidade solicitada.

- **Fonte 1.** Entrevista com o responsável comercial sobre a regra de formação do total. **Fonte humana, nível tático.**
- **Fonte 2.** Consulta à tabela de preços e às regras comerciais vigentes, caso estejam documentadas. **Fonte não humana, categoria documentação.**

### R03 — Identificação do pedido

**Requisito.** Ao salvar um pedido, o sistema deve gerar um número único e apresentá-lo ao vendedor para consulta posterior.

- **Fonte 1.** Entrevista com vendedores para verificar como localizam e acompanham uma venda depois do atendimento. **Fonte humana, nível operacional, classe de usuário vendedor.**
- **Fonte 2.** Análise dos comprovantes ou registros de pedidos utilizados atualmente. **Fonte não humana, categoria documentação.**

## Processo 2 — Cadastrar e remover produtos (administrador)

### R04 — Cadastro de produto

**Requisito.** O sistema deve permitir que o administrador cadastre um produto com código, nome e preço de venda.

- **Fonte 1.** Entrevista com o administrador para identificar quais dados usa ao cadastrar produtos. **Fonte humana, nível operacional, classe de usuário administrador.**
- **Fonte 2.** Consulta ao catálogo ou à lista atual de produtos, se existir. **Fonte não humana, categoria documentação.**

### R05 — Consulta de produtos

**Requisito.** O sistema deve permitir que o administrador localize produtos cadastrados por código ou nome antes de selecionar um deles para remoção.

- **Fonte 1.** Observação ou entrevista com o administrador sobre como identifica o produto correto. **Fonte humana, nível operacional, classe de usuário administrador.**
- **Fonte 2.** Análise de sistemas de cadastro de produtos usados por empresas semelhantes para identificar formas usuais de busca. **Fonte não humana, categoria concorrência.**

### R06 — Remoção do catálogo

**Requisito.** O sistema deve permitir que o administrador retire um produto do catálogo disponível para novos pedidos, mantendo os dados do produto nos pedidos já registrados.

- **Fonte 1.** Entrevista com o administrador para entender o que significa “remover” no processo da empresa. **Fonte humana, nível operacional, classe de usuário administrador.**
- **Fonte 2.** Consulta a pedidos antigos e ao catálogo atual para verificar como produtos descontinuados aparecem no histórico. **Fonte não humana, categoria documentação.**

## Processo 3 — Controlar o estoque (equipe de estoque)

### R07 — Entrada de produtos

**Requisito.** O sistema deve permitir que a equipe de estoque registre a entrada de uma quantidade de determinado produto, aumentando seu saldo disponível.

- **Fonte 1.** Entrevista com a equipe de estoque sobre o recebimento e a conferência de produtos. **Fonte humana, nível operacional, classe de usuário estoquista.**
- **Fonte 2.** Consulta aos comprovantes de recebimento e controles de entrada existentes. **Fonte não humana, categoria documentação.**

### R08 — Saída de produtos

**Requisito.** O sistema deve permitir que a equipe de estoque registre a saída de uma quantidade de determinado produto, reduzindo o saldo disponível, e impedir uma saída maior que esse saldo.

- **Fonte 1.** Entrevista com a equipe de estoque sobre a baixa de produtos e o tratamento de falta de mercadoria. **Fonte humana, nível operacional, classe de usuário estoquista.**
- **Fonte 2.** Consulta aos registros atuais de saída ou separação de mercadorias, caso existam. **Fonte não humana, categoria documentação.**

### R09 — Consulta do saldo

**Requisito.** O sistema deve mostrar à equipe de estoque a quantidade disponível de cada produto, considerando as entradas e saídas registradas.

- **Fonte 1.** Entrevista com a equipe de estoque sobre as informações necessárias para decidir se há produto disponível. **Fonte humana, nível operacional, classe de usuário estoquista.**
- **Fonte 2.** Consulta às planilhas, fichas ou relatórios usados atualmente para conferir o saldo. **Fonte não humana, categoria documentação.**

**Total:** três requisitos para cada um dos três processos. Cada requisito foi relacionado a uma fonte humana e a uma fonte não humana para confrontar o processo relatado com os registros disponíveis.
