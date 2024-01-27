# LED Remote control over WIFI with ESP32s3

## Usage

Following steps are assuming that you know how to compile and run Rust on ESP32. If not please check ['esp-template'](https://github.com/esp-rs/esp-template) and follow those steps to firstly setup simply esp `no_std` application.

1. Install [`cargo-generate`](https://github.com/cargo-generate/cargo-generate)
    ```
    cargo install cargo-generate
    ```
2. Set up a sample project with this template
    ```
    cargo generate --git https://github.com/OakDevices/ESP32-T-Display-S3-Slint-Rust-Template --name my-project
    cd my-project
    ```
3. Run on the Desktop (Simulator)
    ```
    cargo run --features simulator
    ```
4. Run on the target board with
    ```
    cargo +esp run --target=xtensa-esp32s3-none-elf --features=esp32s3 --release
    ```

## Next Steps

We hope that this template helps you get started and you enjoy exploring making user interfaces with Slint. To learn more
about the Slint APIs and the `.slint` markup language check out our [online documentation](https://slint-ui.com/docs/rust/slint/).
