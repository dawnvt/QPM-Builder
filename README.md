# QPM-Builder
Dependency Resolver for Beat Saber Quest mods written in Rust

## cargo.toml layout
```Rust
[package]
name = "my-mod"
version = "0.1.0"
authors = ["me"]
edition = "2021"

[package.metadata.ndk]
targets = ["arm64-v8a"]
platform = 24

[package.metadata.qpm.dependencies]
chroma = "1.0"
coolmod = "0.3"

[lib]
crate-type = ["cdylib"]

[dependencies]
tracing = "0.1"
qpm-builder = "0.1"

[dependencies.quest_hook]
git = "https://github.com/StackDoubleFlow/quest-hook-rs.git"
features = ["unity2019"]```
