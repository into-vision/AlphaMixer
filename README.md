# AlphaMixer
OBS上でクロマキーを使用せずに透明度を指定した動画を再生するツールを作成しました！

通常のフルカラー動画に対して、透明度をモノクロで描いた動画を使って透過させます。
虹色だろうとなんだろうとクロマキーの制限に悩まされずに綺麗な半透明グラデーションが実現出来ます！


# Q&A
Q.このツールはOBSのプラグイン拡張ですか？
A.いいえ。一般的なモダンブラウザ(ChromeとかEdgeとか)で動作するHTMLファイルで実現されています。
　そのためOBSの「ブラウザ」ソースで読み込むだけでご使用いただけます。

Q. このツールは誰でも使っていいのですか？
A.はい。どなたでもご使用いただけます。
　製作者は にじさんじ の 鈴谷アキくん のファンとして活動していますが、
　鈴谷アキくんだけでなく、にじさんじ内外、Vtuber /Youtuber問わず、イベントでも収益化枠であろうといつでも誰でもご使用いただけます。

Q.動画や配信で権利者表記は必要ですか？
A.いいえ。このツールを使った配信/動画/作品に権利者表記は不要です。

Q.ファイルを再頒布する際は別途権利者表記が必要ですか？
A.いいえ。ツール(htmlファイル)内に権利者表記が記述されているのでそれで問題ありません。
　ただし、このツールを同封して動画ファイルを配布する場合は、配布ページまたはツイート(スレッドでも可)に、
　使用方法の案内という形でツイートのリンクまたはツールの配布ページをリンクしていただけると嬉しいです(強制ではありません)
　またツールの内部を変更している場合は変更点を別途わかりやすい場所(配布ページなど)に明記する必要があります。

Q. settings.iniの変更点も明記する必要がありますか？
A.いいえ、便宜上settings.iniのパラメータの変更のみの場合は記述する必要がありません。
　ただし、 settings.iniにスクリプトを追加するなどした場合は明記する必要があります。

Q.なぜ動画を上下につなげているのですか？
A.試作中は2つの動画を別で用意して同時に再生していましたが、HTMLの仕様上再生時間が完全には同期出来なかったためこうなっています。

Q.HTMLファイルですが直接起動した場合では動画が再生されません。
A.仕様です。理由としてはブラウザの制約でJavaScriptから直接ローカルファイルが参照できないためです。
　OBS上のブラウザ機能はその制約が少し緩められているので問題なく再生できます。

Q.どういう技術で動いてますか？
　前述したとおり一般的なモダンブラウザ(ChromeとかEdgeとか)で動作するHTMLファイルで出来ることのみを使用しています。
 具体的には JavaScript と WebGL を使用しており、外部ライブラリなどは使用していません。

# その他
　　扱いとしてはファンメイドのプログラム作品になるかと思います。
　企業所属の方は使用する際は運営さんに使用許可を打診していただき判断に従っていただければと思います。

　　プログラムを精査して頂く場合を考慮して難読化等はしておらずフルコードが記述されています。
　コードはJavaScript/WebGLで記述されており、外部ライブラリなどは使用していません。
　400行未満のコードでコメントもつけていますので査読しやすくしたつもりです。
 
　　またこのツールを使用したファンメイドの動画が配布されていた場合、中に再頒布という形でこのツールが同梱されているかもしれません。
  その場合は運営さんに相談し、そのまま同梱されているツールを使用するのか、念の為公式からダウンロードしたものを使用するのかの判断を仰いでいただければと思います。
  理由としては改ざんを懸念してものとなっています。
 
# 権利者表記など

製作：バイザン
twitter：@into_vision
GIT：https://github.com/into-vision/AlphaMIxer

ライセンス形式：Apache License 2.0
　以下特筆事項
 ・再頒布可能です。
  ただし修正箇所があればそれをreadmeや配布ページなどわかり易い場所に明記する必要があります。
  この際、settings.iniのパラメータの変更点は記載する必要はありません。
  settings.iniにスクリプトを追加するような場合は明記する必要があります。

 ・個人または社内などパブリックではない環境で使用する分にはご自由に変更できます。　
 ・製品に対して義務や責任は負いかねます。
