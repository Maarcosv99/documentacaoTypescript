# Funções

### Tipo de parâmetro

Podemos informar o tipo que queremos receber em cada parâmetro da função.

```typescript
function soma(a: number, b: number) {
  return a + b
}
console.log(soma(2,5))
```

Neste caso a variável `a`e `b` só recebem números inteiros ou flutuantes. Caso receba uma string, irá gerar erro.



### Tipo de retorno

O Typescript não reclama se você não definir o tipo de retorno de uma função, mas é importante que declare.

```typescript
function greeting(name: string): string {
  // A função só pode retornar string
  return `Olá ${name}`
}

console.log(greeting("Marcos"))
```

A função `greeting` retorna uma `string`.



### Funções anônimas

```typescript
setTimeout(() => {
  const sallary: number = 1000
  // console.log(parseFloat(sallary)) Erro, pq parseFloat recebe string
  // console.log(`Salário: ${sallary}`)
}, 0)
```

Se você tentar o `parseFloat(sallary)` irá receber um erro, que o Typescript vai te avisar antes mesmo que você execute.&#x20;



O `parseFloat` recebe uma string como parâmetro, então não aceita variáveis do tipo number dentro dele, porque isto foi declarado.



### Parâmetro opcional

Se colocarmos uma `?` na frente do argumento, estaremos dizendo que ele é opcional e não é obrigatório passar ele na função.

**P.S.:** O primeiro argumento não pode ser opcional.

```typescript
function advancedGreeting(firstName: string, lastName?: string) {
    return `Olá ${firstName} ${lastName}, tudo bem?`
}
```

A função acima dará erro, pois precisamos validar se o parâmetro lastName recebeu algum valor para que assim conseguimos mostrá-lo.

### Validação de parâmetro opcional

```typescript
function advancedGreeting(firstName: string, lastName?: string) {
  if (lastName !== undefined) {
    // Isso é um early return
    return `Olá ${firstName} ${lastName}, tudo bem?`
  }

  return `Olá ${firstName}, tudo bem?`
}

console.log(advancedGreeting("Marcos", "Viana"))
console.log(advancedGreeting("Teste"))
```

