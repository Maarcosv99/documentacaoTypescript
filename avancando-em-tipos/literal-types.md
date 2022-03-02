# Literal Types

É um recurso que permite colocar valores como tipos.

Isso restringe o uso a não só timos, como também os próprios valores.

É muito utilizado com o **Union Types** [union-type.md](union-type.md "mention").

```typescript
let test: "testando"
// test = 1 // Erro pq precisa ser o valor "testando"

function showDirection(direction: "left" | "right" | "center") {
  console.log(`A direção é: ${direction}`)
}

showDirection("left")

type Direction = "left" | "right" | "center"

function showDirection2(direction: Direction) {
  console.log(`A direção é: ${direction}`)
}

showDirection("center")
```

No exemplo acima declaramos que o argumento **direction** só pode recebr os seguintes valores: `left, right ou center`.
