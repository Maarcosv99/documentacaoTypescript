# BigInt

Com o tipo **\`bigint\`** podemos declarar números com valores muito altos.

Podemos utilizar a notação literal, exemplo: 100n

Para este recurso precisamos mudar no `tsconfig.json`a versão para `ES2020`.

```typescript
let n: bigint
// Ele não aceita números como 10, 11, 12.34

n = 1000n // Funciona pq mudei o target para es2020
```
