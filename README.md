# Rust CLI　基礎
## 概要
逆ポーランド記法をファイルまたは、標準入力からの入力をもとに計算結果を出力する。  
引数、テスト、エラーハンドリングなどの基礎的な実装を行っているので新規作成するプログラムの雛形として利用することが目的。

処理内容は下記参考書Capter 4の内容です。  
一部、クレートのバージョンによるもので、本書通り動かない箇所があり。

[実践Rustプログラミング入門](https://www.amazon.co.jp/%E5%AE%9F%E8%B7%B5Rust%E3%83%97%E3%83%AD%E3%82%B0%E3%83%A9%E3%83%9F%E3%83%B3%E3%82%B0%E5%85%A5%E9%96%80-%E5%88%9D%E7%94%B0-%E7%9B%B4%E4%B9%9F/dp/4798061700)

## 利用クレート
- anyhow
- clap

## Usage
```
# ファイル利用の場合
cargo run -- input.txt

# 標準入力の場合(e.g.)
cargo run
1 1 + 2 *

# help
cargo run -- -h
```

## インストール
```
# インストール
cargo install --path .

# アンインストール
cargo uninstall rpncalc
```