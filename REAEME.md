# README

## 学ぶこと
関数型プログラミングの基礎学習のためのプロジェクト。
『プログラミングの基礎』に記載のコードを写経しながら、関数型プログラミングが何か雰囲気を掴むことが目的。

### 2.Ocamlの基本事項

実数の四則演算は+.のように演算子の後ろに.をつけないとできない。
整数と実数の演算は区別されているためできない。
実数には冪乗を求める関数が定義```**```で実行できる。
文字列は```"..."```で定義
文字列の結合は```^```で実行できる
否定演算子は```not```
型推論なので型定義がいらない。
```let 変数名 = 式```で変数を定義。
関数型言語における変数は基本的に書き換えることができない。
``` let 関数名 引数 ... = 式 ```で関数を定義

## 環境構築
### OCamlをMacにインストール

必要なモジュールをインストール。

```
brew install opam
brew install ocaml
brew install hg
brew install darcs
```

OCamlのインストールと初期設定の実施。

```
opam init
```

Ocamlはデフォルトで矢印キーを使えない。
矢印キーをつかえた方が便利なので下記を実施

```
brew install rlwrap
rlwrap ocaml
```

矢印キーが使えるようにエイリアスを設定

```
echo 'alias ocaml="rlwrap ocaml"' >> ~/.bashrc 
source .bashrc
```

エイリアス設定されていることを確認
```
% alias
alias ocaml='rlwrap ocaml'
```

## 対話的実行
下記で対話的に実行できる。抜けるときはControl + D
```
rlwrap ocaml
```
対話時にプログラムを読み込むのは下記のコマンド
```
#use "sample.ml" ;;
```

## プログラムの実行方法
単一ファイルの実行
```
ocaml <ファイル名>
```

## 参照
### 環境構築
https://program-shoshinsya.hatenablog.com/entry/2019/04/09/221148

https://e-tec-memo.herokuapp.com/article/313/

### プログラムの実行方法
https://scrapbox.io/ohbarye/OCaml%E3%83%97%E3%83%AD%E3%82%B0%E3%83%A9%E3%83%A0%E3%81%AE%E5%AE%9F%E8%A1%8C%E6%96%B9%E6%B3%95