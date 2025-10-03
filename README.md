# 📓 The Ultimate React Course 2025

## 00 - Revision Javascript

Nós iremos trabalhar neste capítulo uma revisão de conceitos de Javascript, tais quais:

- Destructuring
- Spread operator
- Template literals
- Ternaries
- Promises
- Async / Await
- Map, filter, reduce, sort

### 📍 Destructuring

```js
const numeros = [10, 20, 30];
```

✏️ Extraindo os valores

```js
const [a, b, c] = numeros;

console.log(a); // 10
console.log(b); // 20
console.log(c); // 30
```

✏️ Pulando elementos

```js
const numeros = [10, 20, 30, 40];
const [primeiro, , terceiro] = numeros;

console.log(primeiro); // 10
console.log(terceiro); // 30
```
