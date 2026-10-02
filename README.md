# trabalho-engenharia-software

Trabalho de Engenharia de Software do Prof Henry em 2026-02

Este repositório é onde vou guardar meu trabalho da disciplina de Engenharia de Software.

## Diagrama UML

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
### Diagrama de Classe

```mermaid
classDiagram
   class Veterinario {
    - nome: string
    - CPF: string
    %% métodos: açôes que serão desempenhadas
    %% por essa entidade no sistema
    +dar nome() string
    +darCPF() string
    +atenderAnimal(animal: Animal) void
  }
  Veterinario -- Animal
  Animal -- Cliente
class Animal{
    - dono: Cliente
    - nome: string
    - raça: string
    - peso: float
    darnome() string
    darraça() string
    darpeso() float

}
class Cliente{
    - nome: string
    - CPF: string
    - endereco: string
    - telefone: string
    - animais: Animal[]

    darnome() string
    darcpf() string
    dartelefone() float
}
```
