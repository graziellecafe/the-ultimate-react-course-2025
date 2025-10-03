# 📓 The Ultimate React Course 2025

## 00 - Building first app React

```js
npm create vite@latest meu-projeto
```

State: Sempre que precisamos que algo mude na interface do usuário, alteramos o estado.

```js
const [advice, getAdvice] = useState("");
```

**useState** é uma função no React que retorna uma matriz. Portanto, como no exemplo, estamos desestruturando a matriz. O primeiro valor temos o estado que chamamos de valor 'advice' e o segundo valor é uma função setter, uma função que utilizamos para atualizar a parte do estado.

Exemplo:

```js
import { useState } from "react";

export default function App() {
  const [advice, setAdvice] = useState("");

  async function getAdvice() {
    const res = await fetch("https://api.adviceslip.com/advice");
    const data = await res.json();
    setAdvice(data.slip.advice);
  }

  return (
    <div>
      <h1> {advice}</h1>
      <button onClick={getAdvice}>Get advice</button>
    </div>
  );
}
```

## 01 - Revision Javascript

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
