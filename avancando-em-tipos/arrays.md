# Arrays

Arrays costumam ter o mesmo tipo e o criamos da seguinte forma:&#x20;

`tipo[]` , ou seja, para:

* string seria `string[]`
* number seria `number[]`
* boolean seria `boolean[]`

```typescript
let numbers: number[] = [1,2,3]
numbers.push(5)

console.log(numbers)

let nomes: string[] = ["Marcos", "Viana"]
console.log(nomes)
```



### Outra sintaxe de Arrays

Também podemos utilizar a interface **Array**, onde o formato da interface é: `Interface<Tipo>`

```typescript
const numbersNewArray: Array<number> = [1,2,3]
console.log(numbersNewArray)
console.log(typeof numbersNewArray)
```



### Any

O any serve para qualquer tipo de variável.

**Devemos evitar ao máximo utilizar any, pois é contra os princípios do Typescript.**

```typescript
const arr1: any = [1, "teste", true, [], {nome: "Marcos"}]
console.log(arr1)
arr1.push([1,2,3])
console.log(arr1)

```

Perceba que a variável `arr1` recebeu uma lista de itens que possui tipos diferentes e isto só foi possível graças ao `any` .
