# GameAction/primolotto

This repository created to play on primolotto website and play grids

## 💻 Usage

Install the package as a dependency from [npm](https://www.npmjs.com/package/@game-action/primolotto):

```bash
npm install @game-action/primolotto
```
or
```bash
yarn add @game-action/primolotto
```


### TypeScript

```typescript
import { Primolotto } from "@game-action/primolotto";

// to connect
const primolotto = await Primolotto.init("email", "password");

// fetch summary information
const summary = await primolotto.summary();
console.log(summary); // Summary { ticket: 187 }

// play grid, max of 10 per day
const grid = await primolotto.playGrid();
console.log(grid); // true or false
```

## 📄 License

- Code: [MIT](./LICENSE) © [Rémy BRUYERE](https://remy.ovh)

<p align="center">
  <sub>An open source project by <a href="https://remy.ovh">rem42</a></sub>
</p>
