# Type Alias x Interface

### Qual escolher?

Na maioria das vezes podemos optar por qualquer um dos recursos sem problemas.



A única diferença é que a Interface pode ser alterada ao longo do código, já o Alias não, ou seja:

* Se pretendemos mudar o tipo no decorrer do código, utilizamos Interface.
* Caso não, utilizamos Type Alias.



É como se o type alias fosse **const** e a interface fosse **let**.



```typescript
interface Person {
  name: string
}

interface Person {
  age: number
}

// const somePerson: Person = { name: "Marcos" } vai dar erro, pq precisa do age
const somePerson: Person = { name: "Marcos", age: 22 }
console.log(somePerson)
```
