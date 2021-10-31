Example show why cxxflags is necessary.

Define `-std=c++17` in cxxflags, no complain from tinygo

```bash
tinygo build -target=./good.json -o test.wasm .
```


Define `-std=c++17` in cflags, show `error: invalid argument '-std=c++17' not allowed with 'C'` error

```bash
tinygo build -target=./bad.json -o test.wasm .
```
