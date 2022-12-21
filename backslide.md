title: backslideがおすすめな理由
title_fotter: backslideがおすすめな理由
class: animation-fade
layout: true


.bottom-bar[
  {{title_fotter}}
  Mt.SQUARE Machida
]

---

class: impact

## {{ title }}

---

# あじぇんだ

### 何がおすすめなのか
### どんなことができるのか
### 簡単な使い方
### その他便利機能

---

# 何がおすすめなのか

プレゼン資料を用意する時にパワポのように凝った機能はなくてもいいんだけど、シンプルかつちょっとおしゃんな感じで作りたい。

--

.center[

そういう時ありますよね？

]

--

.center[

## 少なくとも私はパワポ使えません！

]

--

.center[

そんな時に便利なのが「backslide」になります！

Markdownで書けてRemark.jsがいい感じにやってくれる、そんなツールです。

]

--

- Markdownだから簡単に書ける

--

- LTにちょうどいい

--

- センス不要 (これが一番大事)

---

# どんなことができるのか

--

冒頭でも述べたようにプレゼン資料のようなものを簡単に作ることができます。

以前に「k6」について発表した際にも使用してました。

--

https://github.com/sinedied/backslide

HTMLでのプレゼンかつ、PDFにも変換できちゃいます。


こんな感じ => [backslide / sample](https://sinedied.github.io/backslide/#1)

---

# 簡単な使い方

--

## インストール

backslideをnpmからインストールします。

```sh
npm install -g backslide
```

---

## 使用方法

--

よく使うコマンドだけ

```sh
Usage: bs [init|serve|export|pdf] [options]

Commands:
  i, init                 Init new presentation in current directory
  e, export [files]       Export markdown files to html slides [default: *.md]
  s, serve [dir]          Start dev server for specified dir.  [default: .]
  p, pdf [files]          Export markdown files to pdf         [default: *.md]

...(割愛)
```

---

## テンプレートの作成

--

※ 初回のみ

```sh
bs init --template
```

ディレクトリ内に`presentation.md`というファイルが作成されるので、編集して資料を作成します。

基本的には Markdown記法 で書けますが、remarks.js 用の記法や backslide のテンプレートで用意されている場合もあります。

---

## HTMLへの変換

拡張子が`*.md`のファイルを HTML ファイルに変換します。

```sh
bs e
```

`dist`というフォルダが作成され、その中に`HTML`ファイルが出力されます。

## PDFへの変換

拡張子が`*.md`のファイルを`PDF`ファイルに変換します。

```sh
bs p
```

---

`pdf`というフォルダが作成され、その中に`PDF`ファイルが出力されます。

## プレビュー

ローカルサーバーを起動し、Markdown のライブプレビューを可能にします。

```sh
bs s
```

デフォルトだと`localhost:4100`にアクセスすると`HTML`に変換された状態で確認できます。

---

# その他便利機能

--

- 変数の定義
- ページのクラス属性
- グリッド
- 文字修飾

とかとか。

<br>

--

テンプレートの作成で記載しましたが、`presentation.md`の中に使用できる記法が書かれているので実際に見ながらやるのが手っ取り早いと思います。

---

# おわり

--

Markdownなのでそんなに覚えることもなく軽く用意しないとって時にも便利かな〜といった感じです。

使うコマンドも3つくらいしかないのに全く覚えられません。

---

class: impact

## 以上、ご静聴ありがとうございました。

