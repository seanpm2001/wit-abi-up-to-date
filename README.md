# GitHub Action for `*.wit.md` files

Configured with:

```yml
jobs:
  abi-up-to-date:
    name: Check ABI files are up-to-date
    runs-on: ubuntu-latest
    steps:
    - uses: actions/checkout@v4
    - uses: WebAssembly/wit-abi-up-to-date@v17
```

optionally:

```yml
jobs:
  abi-up-to-date:
    name: Check ABI files are up-to-date
    runs-on: ubuntu-latest
    steps:
    - uses: actions/checkout@v4
    - uses: WebAssembly/wit-abi-up-to-date@v17
      with:
        wit-bindgen: '0.16.0'
        worlds: 'command reactor'
```
