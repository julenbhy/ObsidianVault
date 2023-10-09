#rust #wasm #wasmtime

- Download source from: 
	https://github.com/bytecodealliance/wasmtime/releases
- Modify wasmtime/crates/wasi-threads/src/lib.rs:
	https://github.com/bytecodealliance/wasmtime/blob/main/crates/wasi-threads/src/lib.rs

- Add log using: `log::info!("This is a info log message");
	- Error. The “error” level. Designates very serious errors.
	- Warn. The “warn” level. Designates hazardous situations.
	- Info. The “info” level. Designates useful information.
	- Debug. The “debug” level. Designates lower priority information.
	- Trace. The “trace” level.

- Build from the root of the repository: `cargo build --release


- Run: `RUST_LOG=trace ./wasmtime-modified --wasm-features=threads --wasi-modules=experimental-wasi-threads hello_world.wasm
  [[Run Rust with Logs]]
