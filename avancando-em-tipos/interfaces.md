# Interfaces

### Introdução as Interfaces

Uma outra maneira de nomear um tipo de objeto. Podemos determinar um nome para o tipo e também escolher quais propriedades e o tipo delas.

**É bastante utilizado.**

```typescript
interface Point {
  x: number
  y: number
  z: number
}

function showCoords(obj: Point) {
  console.log(`X: ${obj.x}`)
  console.log(`Y: ${obj.y}`)
  console.log(`Z: ${obj.z}`)
}

const coordObj: Point = {
  x:1,
  y:2,
  z:3
}

showCoords(coordObj)
```
