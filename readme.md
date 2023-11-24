Simple Class for benchmarking in Javascript and Python.

#### Usage Javascript
```js
benchmark
    .it("Some Name", () => {
        ta.hma(close, 10)
    })
    .it("Some Other Thing", () => {
        ta.ema(close, 10)
    })
    // as much as you want it()
    .run(100)
```

### Usage Python
```python
bench \
    .it("EMA", lambda: ta.ema(close, length=10)) \
    .it("HMA", lambda: df.ta.hma(close, 10)) \
    # as much as you want it()
    .run(100)
```