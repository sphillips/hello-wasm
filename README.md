# Test Rust & WASM App

Built with:

- Rust
- [wasm-pack](https://rustwasm.github.io/docs/wasm-pack/)

# Steps to create and build

1. Develop: Add code to `lib.rs`
2. Build: Run `wasm-pack build --target web` from the project root
3. Import and run code in JavaScript:

```
    <script type="module">
      import init, { add } from "./pkg/hello_wasm.js";

      await init();

      console.log(add(1, 2));
    </script>
```

4. Run web server e.g. `python3 -m http.server`
