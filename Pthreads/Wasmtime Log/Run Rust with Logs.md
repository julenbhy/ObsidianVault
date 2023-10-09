#rust 

- By default Rust has the log::Level set to `warn
	- Error. The “error” level. Designates very serious errors.
	- Warn. The “warn” level. Designates hazardous situations.
	- Info. The “info” level. Designates useful information.
	- Debug. The “debug” level. Designates lower priority information.
	- Trace. The “trace” level.

- To enable inferior log levels:
	`RUST_LOG=trace ./test
	or
	`RUST_LOG="warn,test::foo=info,test::foo::bar=debug" ./test



