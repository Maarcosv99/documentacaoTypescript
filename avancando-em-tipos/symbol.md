# Symbol

Funciona somente na versão do **ES2020**.

O Symbol cria uma referência única para um valor, ou seja, mesmo que tenha 2 variáveis com o mesmo valor, quando comparadas, são consideradas diferentes.



Se temos uma variável com o valor "Marcos" e outra variável com o valor "Marcos", através do Symbol, as 2 são diferentes.

```typescript
let symbolA = Symbol("Marcos")
let symbolB = Symbol("Marcos")

console.log(symbolA === symbolB) // false
```
