---
title: SCSS Cookbook
permalink: /documents/scss-cookbook.html
overview:
---

# 概要

本書では SCSS の基本的な機能を解説する。
本書のステータスは Working Draft であり、本書に対するご意見は pull request にてお送りいただきたい。





# 用語

| 用語        | 解説                                                                        |
|------------|----------------------------------------------------------------------------|
| セレクター   | CSS におけるセレクターと同義。スタイルの適用対象を示すもの。                          |
| プロパティー | CSS におけるプロパティーと同義。CSS 仕様にて定義され、スタイルを指定するために使用される。 |





# セレクター操作

SCSS ではセレクターを構造化し、上下関係を明確にすることができる。
@at-root や & を使用することで CSS の構造に捕らわれることのない構造化が可能となる。

また、@extend や @mixin を使用することでスタイルのモジュール化が可能となる。

## セレクターのネスト

SCSS ではセレクターをネストすることができる。
CSS において、ネストされたセレクターは子孫セレクターとして展開される。

###### SCSS

```css
.contents {
  font-size: 10px;
  p, div {
    color: #red;
  }
}
```

###### CSS

```css
.contents { font-size: 10px; }
.contents p, .contents div { color: #red; }
```

## プロパティーのネスト

CSS で同一の名前空間を持つプロパティー(border-、 font-、 text-、 background- など)を名前空間でまとめて定義することができる。

###### SCSS

```css
.contents {
  font: {
    family: sans-serif;
    size: 10px;
    weight: bold;
  }
}
```

###### CSS

```css
.contents {
  font-family: sans-serif;
  font-size: 10px;
  font-weight: bold;
}
```

## 親セレクター参照

SCSS セレクターにおける "&" は親のセレクターに置換される。

###### SCSS

```css
a {
  color: black;
  &:hover {
    color: #red;
  }
  .contents & {
    text-decoration: none;
  }
}
```

###### CSS

```css
a { color: black; }
a:hover { color: red; }
.contents a { text-decoration: none; }
```

## @at-root

"@at-root" を指定されたセレクターはドキュメントルートに移動される。

###### SCSS

```css
.parent {
  @at-root .child { ... }
}
```

###### CSS

```css
.parent { ... }
.child { ... }
```

## @extend

@extend でスタイルを継承することができる。

###### SCSS

```css
.error {
  color: red;
}
.seriousError {
  @extend .error;
  border: 3px solid red;
}
```

###### CSS

```css
.error, .seriousError { color: red; }
.seriousError { border: 3px solid red; }
```

@extend で指定される継承元が存在しない場合、SCSS コンパイル時にエラーが発生する。
継承元が存在しない可能性がある場合は "!optional" を指定することでエラーを回避することができる。

###### SCSS

```css
.seriousError {
  @extend .not-exist !optional;
}
```

## @mixin

mixin を使うことで再利用可能なスタイルを定義することが可能となる。

###### SCSS

```css
@mixin large-text($color:#ff0000) {
  font-size: 20px;
  color: $color;
}
@mixin bordered {
  border: 1px solid #ff0000;
}
.error {
  @include large-text;
  @include bordered;
}
.warning {
  @include large-text(#0000ff);
}
```

###### CSS

```css
.error {
  font-size: 20px;
  color: #ff0000;
  border: 1px solid #ff0000; }

.warning {
  font-size: 20px;
  color: #0000ff; }
```

## @media

@media は CSS 同様に使用できる。

###### SCSS

```css
.sidebar {
  width: 300px;
  @media screen and (orientation: landscape) {
    width: 500px;
  }
}
```

###### CSS

```css
.sidebar {
  width: 300px; }
  @media screen and (orientation: landscape) {
    .sidebar {
      width: 500px; } }
```





# 変数

## 変数の定義

変数の定義には "$" 記号を使用する。変数の使用は "$" 付きで変数名をそのまま記載するか、後述の interpolation を使用する。
同名の変数を複数箇所で定義した場合、コンパイルエラーにはならず定義毎に上書きされる。

###### SCSS

```css
$contents-width: 100%;
$contents-width: 95%;
#contents {
  width: $contents-width;
}
```

###### CSS

```css
#contents { width: 95%; }
```

"!default" を指定することで、既存の変数がある場合は既存を優先させることができる。

###### SCSS

```css
$contents-width: 100%;
$contents-width: 95% !default;
#contents {
  width: $contents-width;
}
```

###### CSS

```css
#contents { width: 100%; }
```

## データ型

SCSS では以下のデータ型がサポートされる。

* 文字列
  * クォーテーションマークの有無は任意。
  * クォーテーションマークはシングル、ダブルのいずれを用いても良い。
  * 例) "foo", 'bar', baz
* 数値
  * 例) 1.1, 10px, 100%, 2em
* 真理値
  * 例) true, false
* 色
  * 例) red, #113355, rgba(255, 255, 0, 0.7)
* リスト
  * セパレーターはスペースもしくはカンマを用いる。
  * 例) 1px 1px 0 2px
  * 例) Helvetica, Arial, sans-serif
* マップ
  * 例) (id: scott, pwd: tiger)
* null

## interpolation

interpolation は "#{" および "}" で表す。
interpolation を使用することで変数をそのまま指定できない箇所(セレクター名など)でも変数を利用できる。
interpolation 内では式を利用することができる。

```css
$id: #contents;
$contents-width: 100%;
#{$id} {
  width: #{$contents-width - 4%};
  padding: 0 2%;
}
```

```css
#contents {
  width: 96%;
  padding: 0 2%;
}
```





# 制御構文

## @if

###### SCSS

```css
$type: "bordered";
p {
  @if $type == "bordered" { border: 1px solid;  }
  @else if $type == "dotted" { border: 1px dotted; }
  @else { border: none; }
}
```

###### CSS

```css
p {
  border: 1px solid; }
```

## @for

###### SCSS

```css
@for $i from 1 through 3 {
  .item-#{$i} { width: 2em * $i; }
}
```

###### CSS

```css
.item-1 {
  width: 2em; }

.item-2 {
  width: 4em; }

.item-3 {
  width: 6em; }
```

## @while

###### SCSS

```css
$i: 1;
@while $i <= 3 {
  .item-#{$i} { width: 2em * $i; }
  $i: $i + 1;
}
```

###### CSS

```css
.item-1 {
  width: 2em; }

.item-2 {
  width: 4em; }

.item-3 {
  width: 6em; }
```

## @each

###### SCSS

```css
@each $color in "red", "blue", "yellow" {
  .item-#{$color} {
    background-color: $color;
  }
}
```

###### CSS

```css
.item-red {
  background-color: "red"; }

.item-blue {
  background-color: "blue"; }

.item-yellow {
  background-color: "yellow"; }
```





# 演算子 / 関数

## 関数の定義

関数の定義には "@function" を使用する。

###### SCSS

```css
$grid-width: 40px;
$gutter-width: 10px;

@function grid-width($n) {
  @return $n * $grid-width + ($n - 1) * $gutter-width;
}

#sidebar { width: grid-width(5); }
```

###### CSS

```css
#sidebar {
  width: 240px; }
```

## 文字列操作演算子

| 演算子 | 処理              | 例              | 備考 |
|-------|------------------|-----------------|-----|
| +     | 文字列の結合       | "abc" + "cde"   |     |

## 数値操作演算子

| 演算子 | 処理              | 例      | 備考  |
|-------|------------------|---------|------|
| +     | 数値の加算         | 5 + 2   |      |
| -     | 数値の減算         | 5 - 2   |      |
| *     | 数値の乗算         | 5 * 2   |      |
| /     | 数値の除算         | (5 / 2) | 除算演算子 "/" は CSS で特殊な意味を持つため要注意。除算として "/" を用いる場合は特定の条件を満たさなければならない。 |
| %     | 数値の剰余算        | 5 % 2  |      |
| <     | 数値の比較(未満)    | 5 < 2   |      |
| >     | 数値の比較(より大)  | 2 > 5   |      |
| <=    | 数値の比較(以下)    | 5 <= 2  |      |
| >=    | 数値の比較(以上)    | 2 >= 5  |      |
| ==    | 数値の比較(一致)    | 5 == 5  |      |
| !=    | 数値の比較(不一致)  | 5 != 2  |       |

## 真理値操作演算子

| 演算子 | 処理              | 例                   | 備考  |
|-------|------------------|---------------------|------|
| and   | 真理値の論理積      | $a == 1 and $b == 2 |      |
| or    | 真理値の論理和      | $a == 1 or $b == 2  |      |
| not   | 真理値の否定       | not $a == 1          |      |

###### SCSS

```css
$theme: "white";
#contents {
  @if $theme == "white" or $theme == "light"  {
    background-color: #FFF;
  }
}
```

###### CSS

```css
#contents { background-color: #FFF; }
```

## 色操作演算子

| 演算子 | 処理      | 例                   | 備考  |
|-------|----------|---------------------|------|
| +     | 色の加算   | #FF0000 + #00FF00   |      |
| -     | 色の減算   | #FFFF00 - #00FF00   |      |
| *     | 色の乗算   | #010203 * #040506   |      |
| /     | 色の除算   | (#060c14 / #020304) | 除算演算子 "/" は CSS で特殊な意味を持つため要注意。除算として "/" を用いる場合は特定の条件を満たさなければならない。 |
| %     | 色の剰余算 | #FFFFFF % #222222   |      |

## リスト操作関数

* [リスト関数](http://sass-lang.com/documentation/Sass/Script/Functions.html#list-functions)
* [@each ディレクティブ](http://sass-lang.com/documentation/file.SASS_REFERENCE.html#each-directive)

## マップ操作関数

* [マップ関数](http://sass-lang.com/documentation/Sass/Script/Functions.html#map-functions)
* [@each ディレクティブ](http://sass-lang.com/documentation/file.SASS_REFERENCE.html#each-directive)

## セレクター操作関数

* [セレクター関数](http://sass-lang.com/documentation/Sass/Script/Functions.html#selector_functions)

## 内部操作関数

* [内部操作関数](http://sass-lang.com/documentation/Sass/Script/Functions.html#introspection_functions)

## その他の関数

* [その他操作関数](http://sass-lang.com/documentation/Sass/Script/Functions.html#miscellaneous_functions)





# @import

SCSS ファイルに他の CSS / SCSS ファイルをインポートする。

###### SCSS

```css
@import "foo.css";
@import "foo" screen;
```

@import はネストさせることも可能。

###### SCSS

```css
// foo.scss
.bar {
  color: red;
}
// main.scss
#main {
  @import "foo";
}
```

###### CSS

```css
#main .bar {
  color: red;
}
```

他の SCSS ファイルで @import されるためだけに作成される CSS / SCSS ファイルを Partial と呼称する。
Partial はファイル名に prefix "_" を付与することで識別され、単体の SCSS としてコンパイルされることはない。

###### SCSS

```css
// _foo.scss
.bar {
  color: red;
}
// main.scss
@import "foo";
```

###### CSS

```css
// main.css
.bar {
  color: red;
}
// _foo.css は出力されない。
```


# ロギング/エラー処理

## @debug

@debug によりデバッグメッセージを出力することができる。

###### SCSS

```css
$width: 100px;
@debug "width is #{$width}";
```

```
Line 2 DEBUG: width is 100px
```

## @warn

@warn により警告メッセージを出力することができる。警告メッセージは "--quiet" オプションで非表示にすることができる。

###### SCSS

```css
$width: 100px;
@warn "width is #{$width}";
```

###### 出力

```
WARNING: width is 100px
         on line 2 of an unknown file
```

## @error

@error によりエラーメッセージを出力し、処理を中断することができる。

###### SCSS

```css
$width: 100px;
@warn "width is #{$width}";
```

###### 出力

```
Error: width is 100px
        on line 2 of standard input
  Use --trace for backtrace.
```





# コメント

SCSS ではシングルラインコメントとマルチラインコメントがサポートされている。

シングルラインコメントは css への変換時に削除される。
マルチラインコメントは「出力スタイル」オプションが "compressed" の場合にのみ削除される。

###### SCSS

```css
/*
 this is multiline comment.
 */
.contents {
  // this is Single-line comment
  font-size: 10px;
}
```

###### CSS

```css
/* this is multiline comment. */
.contents { font-size: 10px; }
```
