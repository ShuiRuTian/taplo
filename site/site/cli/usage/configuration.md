# Configuration

## Log Level

Taplo uses the Rust `tracing` library for configurable logging features and respects the `RUST_LOG` environment variable.

In most cases you might wish to disable logging after a certain log level, for example if you wish to only see error messages, you can do the following:

```sh
RUST_LOG=error taplo lint foo.toml
```

The available log levels:

- `trace`
- `debug`
- `info`
- `warn`
- `error`

## Configuration File

<!-- TODO: config link -->

Taplo CLI by default searches for a Taplo config file in the current working directory, this behaviour can be disabled by either supplying `--no-auto-config` or `--config <path>` flags.