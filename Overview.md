1. Compiling
 <br>
 a. Use binaryen
 <br>
 b. Not tied to runtime/platform (CLI? Pure WebAssembly would be sick)
 <br>
 c. Compile to native via wasm2c or LLVM?
 <br>
 d. Allow user to create compile flags
2. Closures
 <br>
 a. Complete asap
3. Syntax
 <br>
 a. Use bracket-syntax
 <br>
 b. Use optional semi-colon endings
4. Transform
 <br>
 a. Written in core language (Not tied to a runtime)
 <br>
 b. Built in features
  <br>
  I. String to AST parsing?
  <br>
  II. Type reflection?
5. Platforms
 <br>
 a. Platform-neutral
 <br>
 b. WASI default (Polyfill for JavaScript)
7. Async/Await
 <br>
 a. Await can be outside of async function
 <br>
 b. Use asyncify
8. Memory
 <br>
 a. Pointer support
 <br>
 b. Memory copys
 <br>
 c. Memory alloc
 <br>
 d. later
9. WASI
 <br>
 a. Console support
 <br>
 b. Date support
 <br>
 c. FileSystem support
 <br>
 d. Sockets support
 <br>
 e. HTTP support (once released)
10. Server (Lunatic?) WASI
 <br>
 a. --server compile flag?
 <br>
 b. Sockets
 <br>
 c. Threads
 <br>
 d. HTTP
 <br>
 e. WebSockets
 <br>
 f. UDP
 <br>
 g. IPC
 <br>
 h. Native addons? (NAPI/NEON-Like)
11. Performance
 <br>
 a. Allow user to insert and modify WAT?
 <br>
 b. Use wasm-opt
12. String encoding
 <br>
 a. UTF-16 (Seems like WASM is using it)
 <br>
 b. Possibly use flags like `--enable-utf8`
13. Functions
 <br>
 a. Provide options to inline