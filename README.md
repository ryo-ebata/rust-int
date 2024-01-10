# Optimal Int

optimal_int は、Rust で書かれたライブラリで、整数を最適な範囲で表現するための型を提供します。このライブラリは、整数を最小の範囲で表現できる型に自動的に変換します。

## 特徴

- i8 から u128 までの整数型をサポート
- 整数を最小の範囲で表現できる型に自動的に変換
- Int 列挙型を使用して、最適な整数型を表現

## 使い方

```rs
use optimal_int::Int;

let small_int = Int::new(-10);
let large_int = Int::new(4000000000u64);
```

上記の例では、small_int は Int::I8(-10)として表現され、large_int は Int::U32(4000000000)として表現されます。

## ビルド

このライブラリをビルドするには、以下のコマンドを実行します：

```zsh
cargo build
```

## テスト

このライブラリのテストを実行するには、以下のコマンドを実行します：

```zsh
cargo test
```

## ライセンス

このライブラリは MIT ライセンスの下で公開されています。詳細は [LICENSE](https://github.com/ryo-ebata/rust-int/blob/main/LICENSE) をご覧ください。
