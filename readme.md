# Demo RUST Apache Thrift test project

1. cargo build
2. ./target/debug/server
3. ./target/debug/client

Start server

```console
./target/debug/server
```

Server response

```console
binding to 127.0.0.1:9000
```

Start client

```console
./target/debug/client
```

Client response

```console
Hello Allen!
client ran successfully
```

## Install Thrift 0.11.0 on Mac OSX

I tried several way to install the latest Thrift, but none was successful. `Thrift ^0.11.0` is required for `Rust` support.

```console
brew install https://raw.githubusercontent.com/Homebrew/homebrew-core/master/Formula/thrift.rb
```

Then we can use the thrift build command

```console
thrift --out src --gen rs simple_service.thrift
```

This will generate the `/src/simple_service.rs` file.