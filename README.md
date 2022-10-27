# Gs_kadai1_janken_1022_002
じゃんけんアプリ進化版


# 課題1 -じゃんけんアプリ-

## ①課題内容（どんな作品か）

- じゃんけんアプリ進化版 【課題をもとにできる工夫を追加してみました】

## ②工夫した点・こだわった点

【処理】
- 配列を使って、じゃんけんの勝ち負け判定をできるようにしたところがポイントです。
- まず、人間が選択したグー、チョキ、パーにそれぞれ値を代入（0,1,2）し、数値化した。
- 次に、コンピューターがランダム生成した数字に基づくグー、チョキ、パーもそれぞれ同様に値を代入（0,1,2）し、数値化した。
- これにより人間が選択した手札と、コンピューターがランダム生成した手札が数値として比較できる状態になり、最後に差し引きの数字で勝ち負け判定をし、判定数値に基づきIF文を分けて表示した。

- 配列を使わない場合も考えたのですが、①　IF（人間がグーを出した場合）｛以下、分岐｝、　②IF（人間がパーを出した場合）｛以下、分岐｝、　③IF（人間がチョキを出した場合）｛以下、分岐｝、の３通りに同じような分岐式をたくさん書かないといけなくなることが想定されたので、配列を使ってまとめられるならばそのほうが構造化しやすそうだなと思い挑戦しました。
- また、自分は作りたいアプリの応用として、もっと手数が多いもの（洋服の種類など無限にあるもの）を今後、応用的にランダム生成することを想定していたので、なるべく配列やまとめられる処理を使って書いてみたかったので、挑戦しました。

【描画】
- 最低限やりたかった「コンピューターのランダム生成によって手数のグーやパーを画像で切り替えて表示する」というところはなんとか実施できました。
- ここができると、勝敗判定の画像化なども同じ仕組みで動かせるので、応用はしやすかったです。
- あとは前回のHTML,CSSの知識を振り返りながら駆使して、自分のイメージにちかいところまで（全体のページ構造と色、選択したときの挙動など）持っていきました。
- ただ、下記の③番に記載のとおり、できなかったことのほうが今回多かったです！くやしい・・・。


## ③難しかった点・次回トライしたいこと(又は機能)

【処理】
- 課題の要件を満たすものを仕上げるだけでかなりの労力がかかってしまった。仕上げるだけでかなり大変だった。
- 途中、本当に「なにから処理を作ったらよいかわからない」「１つ１つ作ってみてもどれも動かない」「どこが違うのかの見当がつけられない」という状態が数日続き、かなり焦りました。
- 処理をステップに分けて考えて、まずいちばん簡単そうなところから着手する、最初の１つや２つが動くようにできると、できるような気持ちになるのとだんだん少しわかってきて、「こうかな？」と試行錯誤ができる状態になる。その状態でも、なかなか仮説通りに動かないことばかりなので、調べるのに無限に時間がかかったりするが、１つ１つクリアしていくしかないと決めてコツコツすすめるしか無いという感覚を持てた。

【描画】　
- 以下、やりたかったけどできなかったことがたくさんありました。
①クリックイベントによる、画像の切り替えをしたときに、fadeIn/fadeOut的な挙動も一緒につけること。（本当は、コンピューターの手札が選ばれたときに、モワッと画像が表示されるようにしたかった！）
　attrによる画像切り替えと、fadeInの両立。
 サムネイルの切り替え方法などのページを見てトライしたが、最後までうまくいかず時間切れに。
 授業でやったfadeInは、画像切り替えと連動していなかったので、そういった単独では動かせるが、複合になったときに急にどうつなげたらよいかの応用が難しくなってしまうので、用途に応じた応用力も身につけたいと痛感する。

②画像の初期設定をなにもなくして、えらばれたときにだけ表示するなどの挙動。
　これも最後までうまくいかず、最終的に間に合わせで「結果は・・・？」や「？」などの初期表示の画像を別で用意して、最初にそれを表示しておき、クリックイベントで画像を切り替える形にして無理やり形にした。
 形にはなっているものの、理想的にやりたかったことが実現できているわけではないので、しっかり理想を実現するスキルを付けたい。
 
③応用的に、自分の手札を選んだら、トランプのカードのように浮き上がり、モダールウィンドウ的に立ち上がらせる挙動にしたかった。（前回CSSのレスポンシブで習った、ハンバーガーメニューの実装のときのようなイメージ）
ただこちらは全然時間が足らず、try&errorさえも出来なかった。次回に向けて応用していきたい。


## ④質問・疑問・感想、シェアしたいこと等なんでも

 【感想】
- HTML/CSS までと違い、JavaScript、Jquery、あたりが入ってきて超絶急に難易度があがりました。（１対１０くらい…）
- ついていけるようにがんばります・・・！
- まだこれからサーバーサイドとの接続が待っていると思うので、まずはプリセットできるところをJSで書いている状況ですが、ここができていないとサーバーが出てきたときに大変なことになりそうなので、ひとつひとつ身につけたいと思います。
- やりたいことがなかなか思ってる通り動いてくれないジレンマがすごい！！！！！！がんばろ〜〜
- 
