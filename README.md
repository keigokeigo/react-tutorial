# React Tutorial


* 2020-02-11 以下をベースに。
* [今から始めるReact入門 〜 React の基本 - Qiita](https://qiita.com/TsutomuNakamura/items/72d8cf9f07a5a30be048)

* JSX を使うと普通にHTML を書く感覚でJavaScript 内にタグを埋めていくことができる
* Babelとは、簡潔にいうと、JavaScriptのコードを新しい書き方から古い書き方へと変換するツールです。
* webpackとはウェブコンテンツを構成するファイルをまとめてしまうツールです。一番多い使い方は、複数のJavaScriptを1つにまとめることでしょう。

* 変数の取扱について
    * JSX 内にJavaScript で定義した変数を埋め込むには `{変数名}` と記述して埋め込むことができます。

* `Layout` の部分はコンポーネント。コンポーネントにプロパティを渡せる。
```
ReactDOM.render(
  <Hello name="Tanaka" />,
  document.getElementById('root')
);
```

* React のコンポーネント化
    * React はコンポーネント化することで、前回記事のように一つのファイルに全てのコンテンツを含めてしまうのではなく、幾つかのファイルに分けていき再利用性を高めることができます。

* `export default class ...`
    * 外部からアクセスできるようにする。

# JSX

* 「JSXとはなんぞや」 というのを理解するとき 「なんとなくHtml風に書けるJavaScriptの拡張構文」
* さらに踏み込むと、 *我々がJSXを書いているとき、それは実際にはReact.createElementを書いている ということ。*
* 最終的には JSXはJavaScriptに変換される。

# Props

* React のJSX でも同様に各コンポーネントに対してパラメータを渡して使うことができ、そうすることでコンポーネント毎に個別の値の引数を渡すことができるようになります。それをReact のJSX ではProps と呼びます。
