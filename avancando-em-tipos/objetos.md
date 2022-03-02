# Objetos

### Tipos de objetos

Determinamos quais tipos as propriedades que um objeto possui.

**Sintaxe:** `{ prop: tipo, prop2: tipo 2 }` ****&#x20;

```typescript
function passCoordinates(coord: {x: number, y: number}) {
  console.log(`X coordinates: ${coord.x}`)
  console.log(`Y coordinates: ${coord.y}`)
}

const objCoord = {x: 239, y: 548}
passCoordinates(objCoord)
// passCoordinates({x: 239, y: 548 })

const pessoaObj: {name: string, surname: string} = {
  name: "Marcos",
  surname: "Viana"
}
```

### Propriedades opcionais

Nem sempre os objetos possuem todas as propriedades que poderiam possui.

**Sintaxe:** `{ prop?: tipo }` **** quando a propriedade possui uma `?` na frente dele, isso diz que ela é opcional e não é obrigatório declarar ela no objeto.



```typescript
function showNumbers(a: number, b: number, c: number) {
  console.log(`A: ${a}`)
  console.log(`B: ${b}`)
  if (c) {
    console.log(`C: ${c}`)
  }
}

showNumbers(1,2,3)
// showNumbers(4,5) Erro, pq precisa do parâmetro c

function showNumbers2(a: number, b: number, c?: number) {
  console.log(`A: ${a}`)
  console.log(`B: ${b}`)
  console.log(`C: ${c}`)
}

showNumbers2(4,5) // Nesta função, c é opcional, retorna undefined, mas espera a e b
```
