# Hi, I'm Hamza

<samp>
  <a href="https://vectrojs.dev">vectrojs.dev</a> ·
  <a href="https://www.linkedin.com/in/hamza-masood7/">linkedin</a> ·
  <a href="mailto:info@vectrojs.dev">info@vectrojs.dev</a>
</samp>

<br><br>

Full-stack engineer from fintech and POS, where real money moves and nothing gets to break. Now I'm building **Vectro**.

<br>

<a href="https://vectrojs.dev">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="assets/vectro-wordmark-white.svg">
    <img src="assets/vectro-wordmark.svg" alt="Vectro.js" height="64">
  </picture>
</a>

Multi-core SQL and dataframes for JavaScript. It runs on every core in Node, the browser and the edge. Pure JS + WebAssembly, no dependencies.

```js
import { Engine, sql } from 'vectrojs';

const engine = new Engine();                  // uses every core
const orders = engine.readCSV('orders.csv');  // parsed in parallel

sql(`SELECT region, SUM(price * qty) AS revenue
     FROM orders GROUP BY region ORDER BY revenue DESC`, { orders }).toRows();
```

Faster than DuckDB 2.0 on **20 of 20** SQL benchmark queries over 10M rows. At a billion rows:

| 1B rows, read from disk | Vectro | DuckDB 2.0 |
|:--|--:|--:|
| Memory used | **0.37 GB** | 6.6 GB |
| Top 10 rows | **11 ms** | 827 ms |

Source and the npm package (`vectrojs`) are launching soon. Follow along at **[vectrojs.dev](https://vectrojs.dev)**.

## Work

Products I build, where real money moves:

- **[ClubTeq](https://clubteq.com)**: golf course management software. Tee sheet booking, pro shop POS, members, tournaments and QuickBooks sync in one system
- **[Invoteq](https://invoteq.com)**: payment processing and POS for US merchants (restaurants, retail, healthcare)

<br>

<sub><em>"Keep moving forward."</em> (Meet the Robinsons)</sub>
