# so-simple-wasm-test
wasm がどんなものかとりあえず試してみたいんじゃ

# 勉強メモ
[使用リンク](https://www.rust-lang.org/ja/learn/get-started)
## setup
インストール
`curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh`

```log
➜  so-simple-wasm-test git:(main) rustup -V    
rustup 1.27.1 (54dd3d00f 2024-04-24)
info: This is the version for the rustup toolchain manager, not the rustc compiler.
info: The currently active `rustc` version is `rustc 1.81.0 (eeb90cda1 2024-09-04)`
➜  so-simple-wasm-test git:(main) cargo --version
cargo 1.81.0 (2dbb1af80 2024-08-20)
```

## start project & run!
```sh
cargo new hello-rust
cd hello-rust
cargo run
```


### use package
rust ではパッケージのことを`クレート`と呼ぶ

Cargo.toml に 追加してビルド
`cargo build`

コードを書き換えて `cargo run`

# 本題！ wasm を試してみよう！
[参考リンク](https://rustwasm.github.io/docs/book/)
目標 : コンウェイのライフゲームを作る！

## rust のインストール！
上のやつ

## wasm-pack のインストール！
`curl https://rustwasm.github.io/wasm-pack/installer/init.sh -sSf | sh`

## git リポジトリをテンプレートとして Rustプロジェクトを作れるやつをインストール
`cargo install cargo-generate`
