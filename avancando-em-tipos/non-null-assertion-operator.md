# Non null Assertion Operator

Às vezes o Typescript pode evidenciar um erro, baseado em um valor que no momento do código ainda não está disponível, porém sabemos que este valor será preenchido.

Evitamos este erro utilizando o caracteres `!`

```typescript
const p = document.getElementById("some-p")
console.log(p.innerText) // Erro porque não sabe se o elemento será capturado ou se existe
console.log(p!.innerText) //Agora confirmamos que ele vai capturar sim, este elemento.
```
