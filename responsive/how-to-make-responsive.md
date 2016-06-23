# レスポンシブWebデザイン
## レスポンシブWebデザインとは
一つの画面(HTML)を、PC、 タブレット、スマートフォン等多様なデバイスで表示しても適切に見やすく、かつデザインを損なうことなく表示できるように、
HTMLやCSS、あるいやJavaScriptを調整して作成されるWebサイトのデザインのことです。

## どんな利点があるのか
現在、Webページを見ることが出来るデバイスは無数にあります。
そのデバイス毎に対応したWebページを作成することが出来ればそれは望ましいのですが、その作成コストは単純にデバイス数分増えていくことになります。
例えば1ページのWebページを作るのにデバイスが100あったとしたら、100ページ分作成することになると言うことにもなりかねません。

## どのように作成するのか
一般に、Webページの内容はHTMLに記述していきますが、その見た目はcssを使って調整していくのが普通です。
なので、デバイスの画面サイズに応じてcssを切り替えて適切な表示を行うと言う方法をとります。

## レスポンシブWebデザインを採用しているサイト

* [スターバックス](http://www.starbucks.com/)
* [カネボウ](http://www.kanebo-cosmetics.co.jp/)

## 主な技術的要素
### フルードグリッド
フルードグリッドとは、下記にあるグリッドデザインとフルードレイアウトを組み合わせた言葉です。

[Responsive Web Design Grid](http://www.w3schools.com/css/css_rwd_grid.asp)

#### グリッドデザイン
グリッドデザインとは、Webページを格子状に区切り、その格子にそってパーツを配置することによって見た目のバランスを調整するデザイン方法です。
#### フルードレイアウト
フルードレイアウトとは、画面や画面内のコンテナの大きさ（高さや幅）をピクセル値などの絶対値で指定せず、
画面に対する比率（%）で相対値で指定されたレイアウトのことです。

### フルードイメージ
表示している画像のサイズを固定サイズではなく、相対的な指定をして伸び縮みさせて表示しているデバイスにフィットさせるように
する技術です。

### メディアクエリー
CSSでは条件によって使用するCSS自体を切り替えることが出来ます。
これを利用して画面サイズを条件としてサイズごとに適切なCSSを使用する技術です。

メディアクエリの例

```css
@media screen and (max-width: 1000px) and (min-width: 700px) {
    ul li a:before {
        content: "Email: ";
        font-style: italic;
        color: #666666;
    }
}
```

## デザイン方法
### モバイルファースト
モバイルファーストとは、スマートフォンなどの携帯端末で表示可能なデザインを最初に行い、その後より大きな画面（タブレットやPCなど）で表示できるように拡張していく方法です。
モバイルファーストの考え方には色々なメリットがありますが、モバイルのような小さな画面のデザインを最初にすることによって
不要な部品は削ぎ落とさざるをえず、必要最低限の機能について慎重に設計することがやりやすいと言うのが挙げられます。

### Designing in Browser
ブラウザの大きさによってデザインが変わるレスポンシブデザインに限って言えば、
実際にブラウザで表示を確認しながらデザインしていく方法が理にかなっているといえます。
Designing in Browserと言うのはブラウザを使ってデザインするということですが、デザインカンプなどの途中成果物を作成しなくても済み、工数が減ると言うのも大きなメリットの一つです。

### ワイヤーフレーム
デザインの前に、簡単なワイヤーフレームを作成します。
ここには少なくとも主要なコンテンツとその配置を確認出来る程度のものを作成します。
内容は、ターゲットのなるデバイスによりますが、スマートフォン、タブレット、PCの3種類があれば通常は良いでしょう。

ワイヤーフレームの例

![](https://cdn.tutsplus.com/webdesign/authors/ian-yates/wireframe.png)

### 実際に作成してみる
#### デフォルトスタイルのリセット
#### cssの記述
##### 文字コード指定
##### margin, paddingリセット
##### aの下線、リスト要素のマーカーリセット
#### viewport
#### フルードイメージ
#### フォント
margin-bottom: 24px
h1 { font-size: 48px; line-height: 1}
h2 { font-size: 36px; line-height: 1.3333 }
h3 { font-size: 24px; line-height: 1 }
hgroup h2, h4, h5, h6 { font-size: 16px; line-height: 1.5; }
#### marginの相殺
* margin-top と margin-bottomの両方が指定されていてそれが重なる場合には数値の大きい方が採用される
#### ヘッダーの中央揃え
#### ナビゲーションの設定
##### 横並び
##### グラデーション
##### hover
### メディアクエリ


## ツール
[Window Resizer](https://chrome.google.com/webstore/detail/window-resizer/kkelicaakdanhinjdeammmilcgefonfh)
