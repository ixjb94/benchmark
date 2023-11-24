Simple Class for benchmarking in Javascript and Python.

#### Usage Javascript
```js
import { Benchmark } from "./benchmark.js"

const benchmark = new Benchmark("My Console Name")

benchmark
    .it("My EMA", () => {
        ta.ema(close, 10)
    })
    .it("My HMA", () => {
        ta.hma(close, 10)
    })
    // as much as you want it()
    .run(100)
```

### Usage Python
```python
from benchmark import Benchmark

bench = Benchmark("My Console Name")

bench \
    .it("EMA", lambda: ta.ema(close, length=10)) \
    .it("HMA", lambda: df.ta.hma(close, 10)) \
    # as much as you want it()
    .run(100)
```