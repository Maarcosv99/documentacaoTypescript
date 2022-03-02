# Type Alias

### Type Alias

É um recurso que permite criar um tipo e determinar o que ele verifica.

Desta maneira temos uma forma mais fácil de chamá-lo em vez de criar expressões complexas com Union Types, por exemplo.

```typescript
function showId(id: string | number) {
  console.log(`O ID é: ${id}`)
}

showId(1)
showId("200")

// Type alias
type ID = string | number

function showId2(id: ID) {
  console.log(`O ID é: ${id} | Type Alias`)
}

showId2(2)
showId2("300")
```

`type ID = string | number` é o nosso **Type Alias**, onde ao invés de colocar nas próximas variáveis/objetos/argumentos que eles recebem `string | number` colocamos agora `ID` pois o tipo ID, recebe `string | number` .
