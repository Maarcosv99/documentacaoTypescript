# Como os tipos são identificados

O Typescript identifica os tipos de um variável através de 2 formas: **Inference** e **Annotation**.

### Inference

Quando você não informa o tipo, mas o Typescript consegue identificá-lo.

```typescript
const name = "Marcos"
console.log(typeof name) // string
```

### Annotation

Quando você informa o tipo para o Typescript. **É considerado a melhor forma, pois deixa tudo explícito.**

```typescript
const name: string = "Marcos"
console.log(typeof name) // string
```
