# trabalho-engenharia-software

Trabalho de Engenharia de Software do Prof Henry em 2026-02

Este repositório é onde vou guardar meu trabalho da disciplina de Engenharia de Software.

## Dagrama UML

```mermaid
flowchart TD
cliente["🧔‍♂️cliente"]
garçom["🤵‍♀️garçom"]


%% ações
subgraph sistema
 comida["pedir comida"]
 vinho["pedir vinho"]
 end

%% relacionamentos
cliente -- "faz pedido" --- comida
garçom --"recebe pedido" --- comida

vinho -. "estende" .-> comida

```

