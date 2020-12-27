# sablejs
🏖️ The safer and faster ECMA5.1 interpreter written by JavaScript, it can be used:
1. Sandbox(like Figma Plugin Sandbox, but better and easy to use);
2. Mini Program/Game JavaScript dynamic execution;
3. Protect JavaScript source code via AOT compiling to opcode;

sablejs may be the fastest interpreter written by JavaScript ([using v8 benchmark suites](https://github.com/mozilla/arewefastyet/tree/master/benchmarks/v8-v7)):

> Benchmark Enviorment: 
> * Node.js v12.19.0
> * Golang 1.15.6
> * GCC 5.4.0 -O3
> * 2.4 GHz Intel Core i9
> * MacOS Mojave 10.14.6 (18G6032)

|     | sable.js  | sval  | eval5  | quickjs-wasm  | mujs  | otto | goja |
|  ----  | ----  | ----  | ----  | ----  | ----  | ----  | ----  |
| Language  | JavaScript | JavaScript | JavaScript | C + WebAssembly | C | Golang | Golang |
| Richards  | 112 | 29.4 | 25.1 | 347 | 187 | 23.4 | 210 |
| Crypto  | 120 | 28.8 | 21.4 | 412 | 113 | 19.2 | 107 |
| RayTrace  | 297 | 102 | 102 | 512 | 392 | 64.5 | 301 |
| NavierStokes  | 179 | 38.0 | 53.1 | 701 | 109 | 31.4 | 191 |
| Total score  | 164 | 42.5 | 41.3 | 476 | 167 | 30.9 | 190 |
| Baseline  | 1 |  ▼ 2.86 | ▼ 2.97 | ▲ 1.90 | ▲ 0.02 | ▼ 4.30 | ▲ 0.16 |
| File Size(KB)  | 294 | 152 | 134 | 434 | - | - | - |
| Gzip Size(KB) | 43 | 40 | 34 | 245 | - | - | - |

**Current progress:**
1. Except for JSON, other logic has been completed
2. Test262 has been integrated, now covered ~70% cases

It will be coming soon...
