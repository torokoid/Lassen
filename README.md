# Lassen

<html>
<head>

<meta charset="UTF-8">
<meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
<meta http-equiv="X-UA-Compatible" content="IE=EmulateIE10" />
<meta http-equiv="X-UA-Compatible" content="IE=edge">

<!--ここから上はお決まりの定型文です-->


<!--ここからが表現の書式などを決めるcssという部分-->

<style type="text/css">
 p {
color: #000000;
font-size: 1.5em;
 }
 

 .red {color:#ff0000;}
 .grey {color:#ffffff; background:#999999;}
 .snow {color:#fffafa;}
 .yellow {color:#ff0000; background:#ffff00;}
 .blue {color:#0000ff;}
 .white {color:#ffffff; blinking;}
 .waku {border:2px dotted #99cc66;
　　　　　　line-height: 200%;
　　　　　　padding: 10px;}

 
 main {
background-color: rgba(255, 255, 255, 0.5);
}

section {
background-color: rgba(0, 225, 0, 0.3);
}
 

/* 点滅 */
.blinking{
	-webkit-animation:blink 1.5s ease-in-out infinite alternate;
    -moz-animation:blink 1.5s ease-in-out infinite alternate;
    animation:blink 1.5s ease-in-out infinite alternate;
}
@-webkit-keyframes blink{
    0% {opacity:0;}
    100% {opacity:1;}
}
@-moz-keyframes blink{
    0% {opacity:0;}
    100% {opacity:1;}
}
@keyframes blink{
    0% {opacity:0;}
    100% {opacity:1;}
}

#wrap {background:none} /*PC用の背景はオフ*/
	
/*背景を指定する部分*/
body::before {
  content:"";
  display:block;
  position:fixed;
  top:0;
  left:0;
  z-index:-1;
  width:100%;
  height:100vh;
  background:url(IMG.pdf) center/cover no-repeat; /*fixedをトル！*/
  -webkit-background-size:cover;/*Android4*/
  }
	
  
a.p:hover {
    position: relative;
    text-decoration: none;
}
a.p span {
    display: none;
    position: relative;
    top: -0.5em;
    left: 2em;
}
a.p:hover span {
    border: none;
    display: block;
    width: 800px;
}   
 

@media	screen and (min-width: 540px),
	screen and (orientation: landscape) {
   p.note { display: none; }
}

article, aside, details, figcaption, figure, header, hgroup, menu, nav, section {
display: block;
}	

#wrap {
margin:0 auto;
width:970px;
}
	
</style>

<link href="https://cdnjs.cloudflare.com/ajax/libs/lightbox2/2.7.1/css/lightbox.css" rel="stylesheet">

</head>

<body>
<!--<div id="wrap">-->

<h2><p class="note"><span class="white">
  モバイル端末をお使いの場合は、画面を横向きにすると
  より見やすくご覧頂けます。
	</span></p></h2>
<!--ここ上は、ほぼそのまま使います！-->

<!--ぱんくずリスト-->
<p><a href="https://dorikawa.github.io/20210704_Utsunomiya_swim/">2021年宇都宮市民大会</a>><a href="https://dorikawa.github.io/HP_build/">IT関連情報IT関連情報</a>>HPの作り方</p>

<!--QRコードの挿入例-->
<p align="left"> <img src="qr2.png" alt="アクセス用QRコード" width="100">アクセス用QRコード</p>
	

<p align="right"><marquee direction="left" scrollamount="20" width="30%">(^_^)/~hada</marquee></p>

<!--流れ文字の挿入例-->
<h1><span class="yellow"><marquee behavior="alternate">!!! GithubでHPを作ろう !!!</marquee></span></h1>


<!--ここから下が、本体部分-->
	
<div style="background-color:rgba(128,255,255,0.8)"> 
<p>HPの作り方を簡単に説明します。<br>HPというのは大まかにいうと以下の２つの要素で出来ています。<br>１，インターネットにつながったサーバー<br>
２，サーバー内に記載したHTMLソースコード<br>では、この二つを説明していきます。</p>

<br><p>インターネットにつながった立派なサーバーを立ち上げるのは<br>費用面で事業というレベルになってしまうので、<br>パソコンレベル以上のことは個人ではやりません。<br>幸いGithubという会社がサーバーを無料で使わせてくれています。<br><br>なぜ無料かというと、<br>この会社はソフトウエア開発者に共同開発の場を提供することが本業で、<br>インターネットサーバーの提供はそのおまけだからです。<br>一般庶民はそのおまけをありがたく使わせてもらうことにします。<br>ほかの手としてはniftyなどのプロバイダーがHP作成ツールを提供してくれたりしていますが、お決まりの書式に当てはめるだけであまり自由度はありません。</p>

    </div> 

<div style="background-color:rgba(255,255,0,0.6)"> 
<p>では、１，のサーバーの確保です。<br>以下のリンクに飛んでGithubのアカウントを作りますが、ドリームかわちメンバーの皆様は、今見ているこのアカウントをお使いいただいてもかまいません。<br>リンク先のSign inでユーザー：dorikawa, パスワード：doridori2021, で入れます。</p>
<p><a href="https://github.com/" target="_blank" rel="noopener noreferrer">Githubリンクhttps://github.com/</a><br>すでにアカウントをお持ちの場合は、リンクのクリックでご自分のアカウントに飛ぶようです。</p>

	</div>


	
<div style="background-color:rgba(0,255,0,0.5)"> 
<p>１，の続きですが、Githubのアカウント内にリポジトリ（≒HP）を作ります。</p>
<p><h2>では、新しいリポジトリを作ってみましょう。<br>
以下のようにクリックして、</h2></p>
<a href="https://dorikawa.github.io/Lassen/IMG.pdf" data-lightbox="abc"><img src="https://dorikawa.github.io/Lassen/IMG.pdf" alt="サンプル画像" width="900" /></a>
<p><h2>リポジトリの名前を適当に決めて入力、<br>
下の二箇所にチェックを入れます。最後に一番下の緑のボタンを押して作成完了です。</h2></p>
<a href="https://dorikawa.github.io/HP_build/20210709_002.png" data-lightbox="abc"><img src="https://dorikawa.github.io/HP_build/20210709_002.png" alt="サンプル画像" width="900" /></a>

</div>

<div style="background-color:rgba(128,255,255,0.8)"> 
<p><h2>ここからが本番で、README.fileにソースコードを書き込んでいきます。<br>
ただし、初めてでは難易度が高いので、以下のコードをコピペして使います。</h2></p>
<p><h2>リンク先に飛ぶと以下のようなソースコードが開きますが、<br>
実際にいじるのは、黄色の吹き出しがある部分だけです。<br>
背景指定はURLになっていますが、同じリポジトリ内のファイル(アップロード方法は後述)ならファイル名の指定だけでOKです。</h2></p>
<a href="20210714_001.png" data-lightbox="abc"><img src="20210714_001.png" alt="サンプル画像" width="900" /></a>
<a href="20210714_002.png" data-lightbox="abc"><img src="20210714_002.png" alt="サンプル画像" width="900" /></a>
<p><a href="https://raw.githubusercontent.com/dorikawa/20210704_Utsunomiya_swim/main/README.md" target="_blank" rel="noopener noreferrer">サンプルコードへのリンク、別のタブで開きます。</a></p>


<p><h2>以下の操作でリンク先のコードをコピペしますが、作成段階でREADME.fileだったものは、README.meになっています。これの鉛筆マーククリックでソースコードをペーストします。<br>
この段階で市民大会の動画配信したページと同じものができています。</h2></p>

<a href="https://dorikawa.github.io/HP_build/20210709_007.png" data-lightbox="abc"><img src="https://dorikawa.github.io/HP_build/20210709_007.png" alt="サンプル画像" width="900" /></a>
</div>

<div style="background-color:rgba(255,255,0,0.6)"> 
<p><h2>では、肝心のYoutube動画のリンク方法です。<br>
Youtubeを開いて、そこにアップされている動画の閲覧画面下、共有ボタンを押します。</h2></p>
<a href="https://dorikawa.github.io/HP_build/20210709_010.jpg" data-lightbox="abc"><img src="https://dorikawa.github.io/HP_build/20210709_010.jpg" alt="サンプル画像" width="900" /></a>
<p><h2>ダイアログの中、埋め込むを選びます。</h2></p>
<a href="https://dorikawa.github.io/HP_build/20210709_011.png" data-lightbox="abc"><img src="https://dorikawa.github.io/HP_build/20210709_011.png" alt="サンプル画像" width="900" /></a>
<p><h2>
埋め込むで出てきたコードをコピーしてそのまま使います。<br>
専門用語で、iframeと呼ばれている仕組みです。<br>
そのままソースコードの中にペーストするとリンクします。</h2></p>
<a href="https://dorikawa.github.io/HP_build/20210709_012.png" data-lightbox="abc"><img src="https://dorikawa.github.io/HP_build/20210709_012.png" alt="サンプル画像" width="900" /></a>

<p><h2>最初にコピペしたHPのソースコード中段に並んでいるものがこれです。</h2></p>
<a href="https://dorikawa.github.io/HP_build/20210709_013.png" data-lightbox="abc"><img src="https://dorikawa.github.io/HP_build/20210709_013.png" alt="サンプル画像" width="900" /></a>

<p><h2>Githubは動画共有に対応していないので、動画はYoutubeを活用するという訳です。</h2></p>
</div>

<div style="background-color:rgba(0,255,0,0.5)"> 
<p><h2>ここからは、このHPでも多用した静止画像の配置方法です。<br>
最初にPC内にある静止画像をリポジトリにアップします。<br>
(必要な画像を事前に作ってある前提・・・(>_<))<br>
リポジトリ内にアップしてあれば、ファイルネームの指定だけで参照できます。<br>
背景に使う画像も同じ方法でアップします。</h2></p>
<a href="https://dorikawa.github.io/HP_build/20210709_008.png" data-lightbox="abc"><img src="https://dorikawa.github.io/HP_build/20210709_008.png" alt="サンプル画像" width="900" /></a>
<p><h2>アップロード動作が終わったら、緑のボタンを押して静止画の追加完了。</h2></p>
<a href="https://dorikawa.github.io/HP_build/20210709_009.png" data-lightbox="abc"><img src="https://dorikawa.github.io/HP_build/20210709_009.png" alt="サンプル画像" width="900" /></a>
<p><h2>Codeボタンを押した時に見える「＊.png」や「＊.jpg」が静止画像のファイルです。</h2></p>
<a href="https://dorikawa.github.io/HP_build/20210709_014.png" data-lightbox="abc"><img src="https://dorikawa.github.io/HP_build/20210709_014.png" alt="サンプル画像" width="900" /></a>
</div>

<div style="background-color:rgba(128,255,255,0.8)"> 
<p><h2>リポジトリ内の画像を表示するソースコードは、以下になります。</h2></p>
<a href="https://dorikawa.github.io/HP_build/20210709_015.png" data-lightbox="abc"><img src="https://dorikawa.github.io/HP_build/20210709_015.png" alt="サンプル画像" width="900" /></a>
<p><h2>ソースコードをいちいち書くのは面倒なので、自動生成するページを作りました。</h2></p>
<p><a href="https://docs.google.com/spreadsheets/d/1wnsQSTP2Vv3ncIYPWtxRlBZRESRBkq_FD-y8f3Vbwpk/edit#gid=1880997290" target="_blank" rel="noopener noreferrer">ソースコード自動生成ページへのリンク、別のタブで開きます。</a></p>

<p><h2>リンク先のページでは、黄色いセルだけ更新すれば、青い列のコードに全て反映されますので、それをコピペするだけで使えます。<br>
ファイルネームの付け方は、日付＋_＋３桁連番＋拡張子、20210704_001.pngみたいにしてあります。</h2></p>
<a href="https://dorikawa.github.io/HP_build/20210709_018.png" data-lightbox="abc"><img src="https://dorikawa.github.io/HP_build/20210709_018.png" alt="サンプル画像" width="900" /></a>
</div>

<br>
<div style="background-color:rgba(255,255,0,0.6)"> 
<p><h2><marquee scrollamount="16">では、何か変更したら、最下段の緑のボタンを押すのを忘れずに！</marquee></h2></p>
</div>

<div style="background-color:rgba(0,255,0,0.5)"> 
<p><h2>最後にリポジトリに記載したHTMLソースコードをHPとして公開する方法の説明です。<br>
以下の操作で、一般的なURLの表示までたどり着きます。<br>
最初に上段右端のSettingを押します。</h2></p>
<a href="https://dorikawa.github.io/HP_build/20210709_003.png" data-lightbox="abc"><img src="https://dorikawa.github.io/HP_build/20210709_003.png" alt="サンプル画像" width="900" /></a>
<p><h2>下の方にスクロールして出てくる、Check it out here!を押します。</h2></p>
<a href="https://dorikawa.github.io/HP_build/20210709_004.png" data-lightbox="abc"><img src="https://dorikawa.github.io/HP_build/20210709_004.png" alt="サンプル画像" width="900" /></a>
<p><h2>以下の三つのボタンを順番に押します。</h2></p>
<a href="https://dorikawa.github.io/HP_build/20210709_005.png" data-lightbox="abc"><img src="https://dorikawa.github.io/HP_build/20210709_005.png" alt="サンプル画像" width="900" /></a>
<p><h2>変更が更新されるまでしばらく待って、ブラウザの更新ボタン(URLの横にある丸まった矢印)を押すと緑色になるので、そこにあるのがHPとして公開するURLです。<br>
URLのクリックでHPとして開きます。</h2></p>
<a href="https://dorikawa.github.io/HP_build/20210709_016.png" data-lightbox="abc"><img src="https://dorikawa.github.io/HP_build/20210709_016.png" alt="サンプル画像" width="900" /></a>
</div>

<br><br>
<div style="background-color:rgba(128,255,255,0.8)"> 
<p><h2>以上、ちょっと長くなりましたがここまでの作業を順番にこなすと、<br>無料の広告なしHPが作れます。<br>
ここまで読んでいただきありがとうございました！<br><br>
	HPの作り方を細かく知りたい方、<br>良い情報がありましたので以下のリンク先からどうぞ。</h2></p>
	<p><a href="https://sakichin.com/" target="_blank" rel="noopener noreferrer">HTMLやCSSなどの説明サイトへのリンク、別のタブで開きます。</a></p>
	<br>
</div>

<br><br><br><br>
<div style="background-color:rgba(255,255,0,0.6)"> 
<p><h2><marquee scrollamount="16">〜〜〜〜〜〜〜〜ご質問等ありましたら、なんなりとどうぞ！簡単なご質問でしたら答えられます。以下のQRコードをスマホで読みこむとブラウザが立ち上がって、メール作成リンクをクリックすると、torokoid@gmail.com(羽田)宛のメール作成動作に入ります。〜〜〜〜〜〜〜〜</marquee></h2></p>
<p align="left"> <img src="https://dorikawa.github.io/HP_build/qr_mail.png" alt="質問メール作成用QRコード" width="100">質問メール作成用QRコード</p>
</div>

<br><br><br><br><br><br><br><br>

<div style="background-color:rgba(0,255,0,0.5)"> 
<p><h2>最後にそこかしこに出てくるネコですが、<br>
Githubのメインキャラ「オクトキャット」(タコ・ねこ)です。<br>
このHPのQRコード真ん中にも配置してあります。<br>
Net技術者の間ではすでに当たり前のキャラで、グッズも販売されています。<br>
気になる方は、以下のリンクから購入できますので、よろしければどうぞ！</h2></p>
<p><a href="https://thegithubshop.com/" target="_blank" rel="noopener noreferrer">Githubのグッズ販売へのリンク</a></p>
<p><h2>こんなのが売られています。</h2></p>
<a href="https://dorikawa.github.io/HP_build/20210709_017.png" data-lightbox="abc"><img src="https://dorikawa.github.io/HP_build/20210709_017.png" alt="サンプル画像" width="900" /></a>
</div>

<br><br><br><br><br><br><br><br>

	
	
	
	



<div style="background-color:rgba(128,255,255,0.8)"> 
<p>おまけ、ドリームかわち水泳教室、瀧田先生の「森のくるまやさん」リンク</p>
<h2><a href="https://tsunakawa-konpou.com/archives/391" target="_blank" rel="noopener noreferrer">手作り感満載のクルマの木製模型、￥300です。<br>オプション部品は¥200とのこと。</a></h2>
<p><h2>職人さん仕上げの完成見本です。</h2></p>
<a href="20210715_001.png" data-lightbox="abc"><img src="20210715_001.png" alt="サンプル画像" width="900" /></a>

</div>
<!--</div>-->
<!--本体はここまで-->


<!--画面に空白地帯を作って、背景が見えるようにしています-->
<br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br>


<h6>
<p align="right"> <span class="snow">背景は7月初旬の紫陽花！</span></p>
</h6>
<!-- フッタ -->
<footer>
	<span class="white"> 2021/07/15 S.Hada</span>
</footer>

<!--HPにさまざまなJavaScriptを呼び込むための書式-->
<script src="https://code.jquery.com/jquery-1.12.4.min.js" type="text/javascript"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/lightbox2/2.7.1/js/lightbox.min.js" type="text/javascript"></script>

<script type='text/javascript' src='https://torokoid.github.io/shiba/jquery.js?ver=1.12.4'></script>
<script src="https://torokoid.github.io/shiba/jquery.goup.min.js"></script>
<script src="https://torokoid.github.io/shiba/my.js"></script>

<!--HPでPDFを表示させるためのJavaScriptを呼び込むための書式-->
<script src="https://cdnjs.cloudflare.com/ajax/libs/pdf.js/2.9.359/pdf.min.js" integrity="sha512-U5C477Z8VvmbYAoV4HDq17tf4wG6HXPC6/KM9+0/wEXQQ13gmKY2Zb0Z2vu0VNUWch4GlJ+Tl/dfoLOH4i2msw==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>

<script src="https://cdnjs.cloudflare.com/ajax/libs/pdf.js/2.9.359/pdf.js" integrity="sha512-or6dZINrKDVWLBVCUIVHNwEf0qJtwBWvw9Edd/s2QCZYBl9lJgQZZqNQY2ZOWW8tF5Yoq6I8adPpC9ELlY325w==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>

<script src="https://cdnjs.cloudflare.com/ajax/libs/pdf.js/2.9.359/pdf.sandbox.js" integrity="sha512-JITnTSR5NqqK/WHKXRehyF+r/3fK+FhC4jiL5YrlfhpcdPzW/r7kd7Ljv8UfxeRmVbYNFcMb79t2LHJukIh5xw==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>

<script src="https://cdnjs.cloudflare.com/ajax/libs/pdf.js/2.9.359/pdf.sandbox.min.js" integrity="sha512-BF/bWXeDqxI+uMBawd/yOd9hTbQm+1WiDMM1ZKS+WlmaDxGP8pPBbgM4uK4FIzJ+cqtp1+aohgyPI7mC3+2xag==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>

<script src="https://cdnjs.cloudflare.com/ajax/libs/pdf.js/2.9.359/pdf.worker.entry.js" integrity="sha512-6P+RcYYDCxpRwRW5WQBiSXpxjIKI2HpvTxAEXPlpzj+iEU26pAS5PCn6E2iVnRK2bJyzAof5TQyfzafaMJIs3w==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>

<script src="https://cdnjs.cloudflare.com/ajax/libs/pdf.js/2.9.359/pdf.worker.js" integrity="sha512-w4WByro84v4oDeAcMT08XbRfqq1O3aXN62vUu5YrMv9XBJ6uFNGQA373e0sl56S7AobpnxtfMKozoLZNYIVxFA==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>

</body>

</html>
