# ネコから逃げろ！ゲーム

この文書は[阿部 和広](https://x.com/abee2)氏によってScratch 1.4向けにに書かれた[「ネコから逃げろ！ゲームを使ったスクラッチワークショップ」](https://swikis.ddo.jp/abee/77)をScratch 3向けに、[石原 淳也](https://x.com/jishiha)がリミックス(加筆・修正)したものである。

<a href="https://creativecommons.org/licenses/by-sa/4.0/deed.ja"><img src="/by-sa.webp" style="width: 10%"></a>
[CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/deed.ja)にしたがって公開します。

<kbd>←</kbd> で戻る。<kbd>→</kbd> で進む。

---

# ファシリテーターの皆さんへ

ナビゲーションバー(ページの左下にマウスを移動すると表示されます)からプレゼンテーションモードに切り替えると、ワークショップを進行するファシリテーター向けのメモを表示します。

<div class="flex justify-center" style="margin-top: 50px;">
　　<img src="/presenter_mode.png">
</div>

---

# ネコから逃げろ！とは?

プログラミングソフト「[スクラッチ(Scratch)](https://scratch.mit.edu/)を使ってつくることができる、マウスでネズミを操作して、追ってくるネコから逃げるゲームです。

<div class="flex justify-center">
　　<img src="/nekonige.png" style="width: 50%">
</div>

<!--
プログラミングソフト「スクラッチ(Scratch)」を使い、自分でプログラムを組んで、ゲームを作るワークショップ。メモはワークショップを進行するファシリテーター向けに書かれている。このワークショップは初心者を対象に最短で30分、発展を入れて2時間くらいまで対応する。
-->

---

# Scratch の起動

<div class="flex justify-center">
　　<img src="/scratch.png" style="width: 50%">
</div>

<!--
https://scratch.mit.edu/ をブラウザで開きます。
-->

---

# 用語の説明

| 用語 | 説明 |
| --- | --- |
| スプライト | キャラクター(役者)となるオブジェクト |
| カテゴリー | ブロック(命令)の分類 |
| ステージ | スプライトがスクリプトにしたがって動く舞台 |
| ブロックパレット | 選択されたカテゴリーのブロック一覧 |
| スクリプトエリア | スクリプト(スプライトの台本。プログラム)を組み立てる場所 |
| コスチューム | スプライトの見た目を決める絵(衣装) |


---
layout: center
---

# かんたんなプログラミング(ネコ歩き)
---

# プログラミングを始める

<div class="flex justify-center" style="margin-top: 50px;">
　　<img src="/start_program.png" style="width: 50%">
</div>

<!--
全員の状態を一致させるため、ウィンドウの一番上の左の方にある「作る」を選ぶ(これに限らず、「ここ」「そこ」などの指示代名詞はなるべく使わない。指示は一度だけでなく、何度も繰り返す)。ファシリテーターは初期画面(「動き」カテゴリーが選ばれ、スクリプトが空で、ステージの中央にネコがいる状態)になっていることを確認する。
-->

---

# 10歩動かす

<div class="flex justify-center" style="margin-top: 50px;">
　　<img src="/move.png" style="width: 50%">
</div>

<!--
スプライト(ネコ)への最初の命令として、左のブロックがたくさん並んでいるところ(ブロックパレット)から青色の「10歩動かす」のブロックをクリック。

ステージのネコを観察して、どこが変わったかを子供に聞く(ちょっと右に動いた)。

ネコの1歩は1ドットに等しい(必要に応じてドットの意味も説明。プロジェクタ－ならドットを目視できるので、実際に見させても良い)。クリックするたびに10ドット右に進む。

ネコが画面からはみ出すまで何度もクリックさせる(ポイントはわざと面倒な事をさせること)。

見えなくなったら、ネコの尻尾をマウスでドラッグして、ステージの中央に戻す。

ファシリテーターは、子供たちをよく観察して、この時点でドラッグ、クリックが難しそうな子をサポート(その場合もなるべく手出しはせず、説明してその子にやらせる)。
-->
---

# ずっと10歩動かす

<div class="flex justify-center" style="margin-top: 50px;">
　　<img src="/forever.png" style="width: 50%">
</div>

<!--
これでも動かせるけど、指が疲れるので、ネコが勝手に動くようにしたい。そこで、「プログラム」を作る。プログラムは命令を順番に並べたもの。コードと同じ意味。

そのためには、「10歩動かす」のブロックをドラッグして、画面の真ん中(スクリプトエリア)に持ってくる。これだけでは、まだなにも変わらない。ブロックをクリックすると動くだけ。

つぎに、「制御」(上から4番目、オレンジ色)をクリックし、「ずっと」のブロックを真ん中(スクリプトエリア)にドラッグし、「10歩動かす」のブロックをはさむ(近づけるとC字型の口の部分が開く)。

「ずっと」をクリックすると、ネコが勝手に動いて画面からいなくなる。尻尾をドラッグして戻しても、またすぐに動き出す。

動きを止めるには画面右上の赤い八角形のボタン(赤信号)をクリックする。ネコが止まったらドラッグして、ステージの中央に戻す。これで最初のプログラムができた(さきほどの手動操作と対比させる)。

ファシリテーターはそれぞれのステップで子供たちの足並みが揃っているかを常に確認し、遅れていたら適宜サポート。
-->
---

# 緑の旗がクリックされたとき

<div class="flex justify-center" style="margin-top: 50px;">
　　<img src="/green_flag.png" style="width: 50%">
</div>

<!--
赤信号が止まれなら、その隣の緑の旗のボタンをクリックすると動きそうだけど、動かない。

これを動かすには、「緑の旗がクリックされたとき」ブロックを「ずっと」の上に付ける。ブロックをドラッグして近づけると、白いハイライトが表示されるので、そこで離すと合体する。
-->
---

# もし端についたら、跳ね返る

<div class="flex justify-center" style="margin-top: 50px;">
　　<img src="/bounce.png" style="width: 50%">
</div>

<!--
今度は、行きっぱなしのネコが自動的に戻ってくるようにしたい。そのためには、「動き」カテゴリーの「もし端についたら、跳ね返る」ブロックを「ずっと」の中、「10歩動かす」の下に入れる。

緑の旗をクリックするとネコがステージを左右に往復する。
-->

---

# 左右に反転

<div class="flex justify-center" style="margin-top: 50px;">
　　<img src="/direction.png" style="width: 30%">
</div>

<!--
(なにか変なことがないか聞く)ネコが右から左に進むとき、ひっくり返るのが変なので、画面右下、「向き」の下のテキストボックスをクリックし、真ん中の「◀|▶」(左右に反転するだけ)ボタンをクリックする。
-->
---

# 次のコスチュームにする

<div class="flex justify-center" style="margin-top: 30px;">
　　<img src="/next_costume.png" style="width: 50%">
</div>

<!--
(まだ変なことがないか聞く)よく見ると、ネコの足が動いていない。これを動くようにしたい。

まず、赤信号をクリックして動きを止める。

画面左上、「コード」の右に「コスチューム」というタブがある。これをクリックするとスクリプトエリアが切り替わり、ネコの絵が2枚表示される。これがネコの衣装(コスチューム)。絵のアイコンをクリックすると、ステージのネコの絵が切り替わる。この切り替えを高速で行えば、パラパラマンガのように、足が動いて見えるのではないか。

「コード」タブをクリックして画面を戻し、カテゴリーを「見た目」(左の上から2段目。紫色)に切り替え、「次のコスチュームにする」ブロックをクリックしてみる。すると、ネコの絵が切り替わる。つまり、このブロックをスクリプトの「ずっと」のなかに入れれば、動いて見えるはず。「次のコスチュームにする」を画面の真ん中(スクリプトエリア)にドラッグして、「ずっと」の中、「もし端についたら、跳ね返る」の下に付ける。

緑の旗をクリックすると足を動かしながらネコが動き始める。
-->
---

# 向きを変える

<div class="flex justify-center" style="margin-top: 20px;">
　　<img src="/change_direction.png" style="width: 30%">
</div>

<!--
ネコが左右に動くだけでは面白く無いので、ステージ全体を動きまわるようにしたい。そのためにはネコの向きを変えれば良い。画面右下、「向き」の下のテキストボックスをクリックして表示される吹き出しのなかの矢印がネコの向きを示しているので、この矢印をドラッグしてネコの向きを変える。
-->
---
layout: center
---

# ネコから逃げろ！ゲームのつくり方　
---

# ネズミのスプライトを追加する

<div class="flex justify-center" style="margin-top: 50px;">
　　<img src="/mouse.png">
</div>

<!--
ネコを動かすことができたので、このネコから逃げるゲームを作る。ネコから逃げるものといえば(参加者に問いかける)、やっぱりネズミなのでそのキャラクター(スプライト)を新しく登場させる。

そのためには、スプライトエリアの右下の「スプライトを選ぶ」(ネコとその右上にプラスマークがついたアイコン)をクリックする。

「スプライトを選ぶ」画面が開いたら、検索フィールドの右「すべて」の横の「動物」を選び、続いて下にスクロールさせて「Mouse1」をクリックしてから「OK」ボタンをクリックする。するとステージにネズミが現れる(「でかい」というリアクションが返るはず)
-->

---

# ネズミの大きさを小さくする

<div class="flex justify-center" style="margin-top: 30px;">
　　<img src="/mouse_size.png" style="width: 60%">
</div>

<!--
ネズミがちょっと大きすぎるので小さくする。スプライトエリアのMouse1が選ばれているのを確認して、「大きさ」の下のテキストボックスをクリックする。数字を100より小さくすればもとの大きさより小さくなる。50くらいがちょうどよい。
-->

---

# ネズミの動きをプログラムする

<div class="flex justify-center" style="margin-top: 30px;">
　　<img src="/mouse_program.png" style="width: 40%">
</div>

<!--
ネズミの動きをプログラムする。ほぼ同じプログラムになるので、ネコのプログラムをまねしてひとつひとつブロックをつなげていくのもよいが、今後も使うことを考えてプログラムをほかのスプライトにコピーする技を教える。

スプライトエリアでネコをクリックし、ネコのプログラムを表示する。「緑の旗がクリックされたとき」の上部あたりにマウスカーソルを乗せ、プログラム全体をつかんで、スプライトエリアのネズミのところまでドラッグする。マウスカーソルがちょうどネズミの上に乗るあたりで、スプライトがぶるぶるっとふるえる動きをするので、ちょうどその場所で離すとコピーすることができる。

緑の旗をクリックするとネズミも足を動かしながら動くことを確認する。

ネズミは自分のキャラクター(自キャラ)なので、コントロールできるようにしたい。ここでは、マウスの操作でステージの中を動かせるようにしてみる。動かすのだからそのブロックは「動き」カテゴリーにあるはず。切り替えると上から9番目に「マウスのポインターへ向ける」というブロックがある。マウスのポインターとはマウスの矢印、カーソルのこと。このブロックを「ずっと」の中、「次のコスチュームにする」の下にドラッグしてはめる。これでよさそうなので、緑の旗をクリックしてみる。ネコが動き、ネズミをマウスでコントロールできる。
-->

---

# ネズミがネコに捕まるとはどういうことか？

<div class="flex justify-center" style="margin-top: 50px;">
　　<img src="/capture.png">
</div>

<!--
しかし、ネズミがネコに捕まってもなにも起こらない。そこはまだプログラムしていないから。次にそれをプログラムする。その前に、ネズミがネコに捕まるとはどういうことか考える(問いかけ)。赤信号で止めてから、ステージ上のネコとネズミが離れた位置にドラッグしてみる。これは捕まっていない。次に、ネコとネズミが重なった(触れた)状態にしてみる。これは捕まっている。つまり、ネコとネズミが触れているかどうかを調べることができれば、捕まったかどうか分かる。それには「調べる」カテゴリーのブロックを使う。
-->

---

# (オレンジ)色に触れた

<div class="flex justify-center" style="margin-top: 20px;">
　　<img src="/orange.png" style="width: 40%">
</div>

<!--
ブロックは沢山あるけれども、ここではネズミから見た時のネコの色(オレンジ色)に注目し、上から2番目の「■色に触れた」を使う。■をクリックすると、色を選択できる吹き出しが表示される。吹き出しの中、3種類のスライダの下にスポイトのアイコンがあるので、それを選択すると、ステージエリアがハイライトされる。ステージの中のマウスがあたっている部分の色を吸い取ることができるようになった。ネコの（白い部分ではなく）オレンジ色の上でクリックする。すると、その色が吸い取られて■の色がオレンジに変わる。

このブロックをスクリプトの中で使いたいけれども、このブロックは両端が尖った六角形なので、はめられる場所がない。それなので、とりあえず真ん中のスクリプトエリアにドラッグしておく。
-->

---

# すべてを止める

<div class="flex justify-center" style="margin-top: 20px;">
　　<img src="/stop_all.png" style="width: 45%">
</div>

<!--
次に、ネコがネズミに捕まったとき(触れたとき)にどうなるか考える(問いかけ)。そのときは、ゲームが終了、つまり、ゲームオーバーになる。ゲームオーバーはゲームが止まって、操作しても動かなくなる状態のこと。赤信号のボタンを押した時と同じ。これを代わりに押してくれるブロックを使えば良い。「制御」の下の方にある「すべてを止める」がそれ。これもまだはめられる場所がないので、とりあえず真ん中のスクリプトエリアにドラッグしておく。
-->

---

# もし〜なら

<div class="flex justify-center" style="margin-top: 20px;">
　　<img src="/if.png" style="width: 45%">
</div>

<!--
これで必要なブロックが揃ったので、これらをつなぎたい。そのためのブロックはないだろうか。そこで、左に並んでいる制御のブロックをみてみると、六角形の穴が開いたブロックがいくつかある。その中でも、「もし〜なら」というブロックが使えそうだ。これも真ん中の灰色の空いているところにドラッグする。
-->

---

# もしオレンジ色に触れたなら、すべてを止める

<div class="flex justify-center" style="margin-top: 20px;">
　　<img src="/if_orange_stop_all.png" style="width: 45%">
</div>

<!--
「もし〜なら」の六角形の穴に「■(オレンジ)色に触れた」をドラッグしてはめる。すると、「もし■(オレンジ)色に触れたなら」になる。続いて、「すべてを止める」を「もし■(オレンジ)色に触れたなら」の開いた口にはめる。すると、「もし■(オレンジ)色に触れたなら、すべてを止める」となる。
-->

---

# 全部のブロックを合体

<div class="flex justify-center" style="margin-top: 20px;">
　　<img src="/mouse_code.png" style="width: 40%">
</div>

<!--
ここまでできたら、全部のブロックを合体させる。「もし■(オレンジ)色に触れたならすべてを止める」の「もし」あたりをつかんでドラッグして、「ずっと」の中の一番下にはめる。コード全体を読むと、「緑の旗がクリックされたとき、ずっと、(いろんなことをしたあと)、もし■(オレンジ)色に触れたなら、すべてを止める」となる。これでネズミのコードは完成した。
-->

---

# 遊んでみよう

<div class="flex justify-center" style="margin-top: 20px;">
　　<img src="/play.gif" style="width: 50%">
</div>

<!--
さっそく、緑の旗をクリックして遊んでみよう。ネコに捕まらないようにマウスを操作してネズミを動かす。ネコに捕まると全体が止まる(ゲームオーバー)。再開するには再度緑の旗を押す。(遊ぶ時間は数分程度。状況を見て判断)
-->

---

# ネコを増やす

<div class="flex justify-center" style="margin-top: 20px;">
　　<img src="/duplicate.png" style="width: 40%">
</div>

<!--
これが簡単すぎるようなら、ネコを増やすと良い。ネコは複製(影分身)できる。スプライトエリアのネコの上で右クリックして「複製」を選ぶと、ネコが増える。ネコの数は全部で2匹から3匹がおすすめ。それ以上だと、難しくなりすぎる。(同じく遊ぶ時間は状況を見て判断)
-->

---

# ネコの速さを変える

<div class="flex justify-center" style="margin-top: 40px;">
　　<img src="/change_speed.png">
</div>

<!--
また、それぞれのネコの速さを変えても良い。変えたいネコをスプライトエリカの上で選んでから、スクリプトの「10歩動かす」の数字をクリックして、キーボードから数字を入力し、最後にEnterキーを押すと、そのネコの速さが変わる。またスクリプトエリア右上に表示されている「向き」の値を変えると、そのネコの向きが変わる。複数のネコの動きを別々にすると難しくなる。(同じく遊ぶ時間は状況を見て判断)
-->

---

# 背景を変える

<div class="flex justify-center" style="margin-top: 40px;">
　　<img src="/stage.png" style="width: 30%">
</div>

<!--
ステージが真っ白でさびしいので、背景をつけてみる。左上の「背景」のタブを選んだ後、左下の「背景を選ぶ」アイコンをクリックする。「背景を選ぶ」画面に表示された背景の中から好きな背景をクリックして選ぶと、その背景がステージにセットされる。
-->

---

# 発表モード

<div class="flex justify-center" style="margin-top: 40px;">
　　<img src="/presentation.png" style="width: 50%">
</div>

<!--
このゲームで遊ぶには、ステージを全画面にするとよい。それにはステージの右上にある4つの矢印が外側に向いたボタンをクリックする(発表モード)。この状態で緑の旗をクリックすると全画面でゲームがスタートする。発表モードを抜けるには、右上の4つの矢印が内側に向いたボタンをクリックする。(遊ぶ時間は状況を見て判断)
-->

---

# プロジェクトの保存

<div class="flex justify-center" style="margin-top: 40px;">
　　<img src="/save.png" style="width: 50%">
</div>

<!--
せっかく作ったゲームもスクラッチを終了したり、パソコンのスイッチを切ると消えてしまう。そうならないように保存する。「ファイル」メニューから「コンピューターに保存する」を選ぶと「Scratchのプロジェクト.sb3」というファイル名で保存される。ファイル名は、本来はその作品に合った名前を付けるべきだが、ワークショップでは、日付、ニックネーム、下の名前など、統一したルールを決めておくとスムーズ。その際、個人情報に留意すること。

キーボード入力は、なるべく自力でやらせるようにするが、どうしても難しい子は手伝う。ファイル名は紙に記録させ、持ち帰って自宅や学校などで続けられるようにする。

保存したプロジェクトは「ファイル」メニューの「コンピューターから読み込む」から再び開くことができる。
-->

---

# 改造タイム

<div class="flex justify-center" style="margin-top: 40px;">
　　<img src="/plus.png" style="width: 50%">
</div>

<!--
この後、時間が余れば、キャラクターの絵を描きかえたり(コスチュームタブのペイントボタン。色に注意)、効果音を入れたり(音タブの録音や読み込みボタン)、スコアやタイマーを追加したりする(「変数」カテゴリー)。何をやるかは状況(子供たちの関心やノリ)で判断する。
-->

---

# スコア

<div class="flex justify-center" style="margin-top: 40px;">
　　<img src="/score.png" style="width: 50%">
</div>

<!--
スコアを作るには、一番右下のステージエリアの「背景」クリックしてから、「変数」カテゴリーの「変数を作る」ボタンで「スコア」を追加する。変数関連のブロックが自動的に増え、ステージに「スコア」が表示される。
-->

---

# スコアのコード

<div class="flex justify-center" style="margin-top: 40px;">
　　<img src="/score_code.png" style="width: 40%">
</div>

<!--
「緑を旗をクリックしたとき」「ずっと」をつないだ基本のスクリプトを作り、「変数」に戻って、「スコアを0にする」を「緑を旗をクリックしたとき」と「ずっと」の間に入れる。「スコアを1ずつ変える」と「1秒待つ」を「ずっと」の中に入れる。

こうすることで、ゲームがスタートしてから1秒逃げ切れるごとに1点が加算されるゲームができあがる。
-->

---
layout: center
---

# 作品の共有

---

# アカウントの作成

<div class="flex justify-center" style="margin-top: 40px;">
　　<img src="/join.png" style="width: 40%">
</div>

<!--
アカウントを作成しサインインすれば、作品は自動で保存されるようになり、「私の作品」の一覧画面からいつでも作品を呼び出せるようになって便利である。ただしScratchのアカウントを作るということは、コミュニティーの一員になることを意味する。保護者と一緒にコミュニティーガイドラインを読み、理解し、守ることをよく説明する。
-->

---

# 共有、使い方やメモ、クレジット

<div class="flex justify-center" style="margin-top: 40px;">
　　<img src="/description.png" style="width: 70%">
</div>

<!--
プロジェクトページの右上「共有」ボタンをクリックすれば、完成した作品をインターネットで共有し、誰でもブラウザーから遊べるようになる。

「使い方」にゲームの操作方法などその作品の利用方法（どのキーを押すなど）を書いておくと、他の子が遊びやすくて親切である。

「メモとクレジット」には、どうやってこのプロジェクトを作成したのか？などのメモや、後述するリミックスをおこなった場合は、その作者への感謝や、どの部分を変更したのかなどを書いておくと良い。

共有した作品は、自分のだけでなく、他の子の作品でも遊ぶように促す。
-->

---

# リミックス

<div class="flex justify-center" style="margin-top: 40px;">
　　<img src="/remix.png" style="width: 50%">
</div>

<!--
共有された他の人の作品は、「中を見る」でどのように作られているかその仕組みを知ることができたり、「リミックス」で直したりできる。変更したもの(リミックス)は再度共有できる。公開されたスクラッチ作品のライセンスははCC BY-SA(クリエイティブコモンズ 表示-継承)なので、他の人の作品をリミックスしてもよい(むしろそうすべき。パクリや盗作ではないことをきちんと説明する。詳細は「よくある質問」の[リミックスとコピー](https://scratch.mit.edu/faq#remix)の更を参照)。
-->

---
layout: center
---

<a href="https://creativecommons.org/licenses/by-sa/4.0/deed.ja"><img src="/by-sa.webp" style="width: 10%"></a>
この文書は[CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/deed.ja)にしたがって公開します。

Markdown形式だけで書ける[Slidev](https://ja.sli.dev/)というツールを使って作っており、GitHub(https://github.com/champierre/nekonige)でソースを公開しています。

リミックス、間違いの指摘、改善提案など歓迎します。
