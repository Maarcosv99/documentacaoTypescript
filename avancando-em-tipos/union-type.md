# Union Type

### Introdução a Union Types

É uma alternativa melhor do que o **any** onde podemos determinar dois tipos para um dado.

**Sintaxe:** `const name: string | null` **** ou seja, a variável name pode receber uma string ou nada (null).

```typescript
function showBalance(balance: string | number) {
  console.log(`O saldo da conta é R$ ${balance}`)
}

showBalance(10)
showBalance("500")

const arr2: Array<number | string | boolean> = [true, 1, "teste"]
```

O argumento balance da função, pode receber uma string ou number.

O arr2 pode receber um array do tipo **number, string ou boolean**.



### Avançando em Union Types

Podemos utilizar condicionais para validação do tipo de Union Types, com isso é possível trilhar rumos diferentes baseado no tipo de dado.

Para checar o tipo, utilizamos o `typeof`

```typescript
function showUserRole(role: boolean | string) {
  if (typeof role == "boolean") {
    return "Usuário não aprovado"
  }

  return `A função do usuário é: ${role}`
}

console.log(showUserRole(true))
console.log(showUserRole("admin"))
```
