# WASM experiments

```shell
# for emcc
brew install emscripten
# wat2wasm
brew install wabt

emcc hello.c -o hello.wasm

curl https://wasmtime.dev/install.sh -sSf | bash
#OR
brew install wasmtime
# new shell after install!
wasmtime hello.wasm


wat2wasm answer.wat -o answer.wasm
wasmtime --invoke answer answer.wasm
```