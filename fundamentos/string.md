# String

Declarando variáveis do tipo `string` para ter acesso a métodos como `.toUpperCase()`

```
const firstName: string = "Marcos"
console.log(firstName.toUpperCase())

let fullName: string

const lastName: string = "Viana"

fullName = `${firstName} ${lastName}`
console.log(fullName) // Marcos Viana

console.log(typeof fullName) // string
```
