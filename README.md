# cargo-license

[![CI](https://github.com/onur/cargo-license/workflows/CI/badge.svg)](https://github.com/onur/cargo-license/actions?workflow=CI)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/onur/cargo-license/master/LICENSE)
![Minimum Supported Rust Version](https://img.shields.io/badge/rustc-1.34-red)

A cargo subcommand to see license of dependencies.

## Installation and Usage

You can install cargo-license with: `cargo install cargo-license` and
run it in your project directory with: `cargo license` or `cargo-license`.

```
cargo-license 0.5.0
Cargo subcommand to see licenses of dependencies.

USAGE:
    cargo license [OPTIONS]

OPTIONS:
    -a, --authors                      Display crate authors
        --all-features                 Activate all available features
        --avoid-build-deps             Exclude build dependencies
        --avoid-dev-deps               Exclude development dependencies
        --color <WHEN>                 Coloring [possible values: auto, always, never]
        --current-dir <CURRENT_DIR>    Current directory of the cargo metadata process
    -d, --do-not-bundle                Output one license per line
        --direct-deps-only             Output information only about the root package and don't
                                       fetch dependencies
        --features <FEATURE>           Space-separated list of features to activate
        --filter-platform <TRIPLE>     Only include resolve dependencies matching the given
                                       target-triple
    -h, --help                         Print help information
    -g, --gitlab                       Gitlab license scanner output
    -j, --json                         Detailed output as JSON
        --manifest-path <PATH>         Path to Cargo.toml
        --no-default-features          Deactivate default features
        --root-only                    Output information only about the root package
    -t, --tsv                          Detailed output as tab-separated-values
```

## Example

`cargo-license` running inside the cargo-license project directory:

![cargo-license](https://i.imgur.com/9KARkwP.png)
