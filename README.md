<div align="center">

  <h1><code>dywapitchtrack-rust</code></h1>

  <strong>Dynamic Wavelet Algorithm Pitch Tracking ported to rust as wasm using <a href="https://github.com/rustwasm/wasm-pack">wasm-pack</a>.</strong>
</div>

## 🚴 Usage

### 🛠️ Build with `wasm-pack build`

```
wasm-pack build --release --target web
```

### 🔬 Use in your project

```
import init, { DywaPitchTracker } from 'dywapitchtrack'

await init()
let dywa = new DywaPitchTracker()

dywa.compute_pitch(audioBuffer, startSample, sampleCount)
```

## 🔋 Batteries Included

* [`wasm-bindgen`](https://github.com/rustwasm/wasm-bindgen) for communicating
  between WebAssembly and JavaScript.
* [`console_error_panic_hook`](https://github.com/rustwasm/console_error_panic_hook)
  for logging panic messages to the developer console.