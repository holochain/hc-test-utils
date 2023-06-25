# hc-test-utils
A library of test utility crates that support testing with Holochain beta releases 0.2.0.

### Usage
This module is has been designed to be included in other Rust codebases as a testing utilty for Rust tests that interface with Holochain.

### List of available crates

- `hc_setup` : This crate contains all the necessary test helpers to spin up holochain, the conductor interfaces,lair keystore. 
    Note: 
        - It will create local temporary configuration files for both the conductor and keystore. 
        - It also contains helper functions to download happ files and storing them locally or create a local mem-proof storage file as a temporary cache when managing cell installation.

## Installation and usage

### Including a `hc-test-utils` crate in your Rust applicaton:

1. Add the following to your `Cargo.toml`:

```toml
[dependencies]
<CRATE_NAME> = {git = "https://github.com/holo-host/hc-test-utils", branch = "main", package = "<CRATE_NAME>"}
```

2. Compile your code anew with the usual `cargo build`.
