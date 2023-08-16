# OneTagger Android

Repository for Android port of [OneTagger](https://github.com/Marekkon5/onetagger)

## Compiling

Requires: Flutter and Rust

```sh
rustup target add aarch64-linux-android armv7-linux-androideabi i686-linux-android x86_64-linux-android
cargo install flutter_rust_bridge_codegen
cargo install cargo-ndk
cargo install cargo-expand

flutter pub get
./build.sh
flutter build apk --release --split-per-abi
```