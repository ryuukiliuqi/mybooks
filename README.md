◎検討技術
アーカイブをカテゴリー毎にレイアウト（デザイン）を変える　	　　https://www.brainsha.co.jp/blog/web/20190524_web2/
Bootstrap4.5  中国語　							https://v4.bootcss.com/docs/getting-started/introduction/
Font Awesome
※ bootswatchでデザイン選択できる
	https://bootswatch.com/cosmo/


◎検討デザイン
　web設計など　　　　										http://hao.shejidaren.com/
  CodeMirror＜HomePageでエディター編集　今後検討＞			https://sumiretool.net/article/d/web_app_tips/codemirror
  Carbonのようにソースコードにシンタックスハイライトを付けて画像化		https://applech2.com/archives/20190806-codeimg-io-create-and-share-source-code-image.html
  
  参考重要　　　　https://jsfiddle.net/3b2r1koL/6/


◎WordPress検討
　Code Syntax Block を検索　



◎概要
　--スケジュール
　　 --7月　簡単なWordPress作成
			　--自分テーマ作成
				 ・基本のSEO機能
				 ・コード表示機能
				 ・基本テーマで作成し、後デザインを変更

  --記事
	 ・サーバー(18件) 修正が必要
	 ・HTML(15)
	 ・CSS(15)
	 ・PHP(15)
	 ・bootstrap(15)
	 ・WordPress(15)
	 ・IOS
	 ・ネットワーク?


		

7
15-30
最低限ワークが作成完了する、今後随時に修正する

15-16 各ページのデザイン検討
17-18 Wordpressへ変更 
19-20 機能追加 

CSS記事を書く？　（１週間？）
本を探す。













ーーーーーーーーーーーーーーーーーーーーーーーーーーーー

まとめ 動的なボタンを実装する際に検討しよう
今回は、●●●●●●●●●●●●についてご紹介しました。

 
利用頻度は低いかもしれませんが、他にもクリック毎に２つの状態を交互に切り換えるボタンやボタンをチェックボックス化したり、ラジオボタン化する方法もあります。
 

まずはサンプルのコードをコピー&ペーストして、文言を変えたり微調整しながら覚えていってみてください。
 

今回は以上になります。最後までご覧いただきありがとうございました。








Demoサイト：https://risethemes.com/downloads/bizline-clean-elegant-theme/
========================================================================



ーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーー
目次

１．テーマに必要な最低限のテンプレートを作成
２．style.cssの説明

ーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーー


ーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーー
１．テーマに必要な最低限のテンプレートを作成
ーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーー
１．テーマに必要な最低限のテンプレートを作成
functions.php
index.php
single.php
header.php
footer.php
style.css

サイトにサイドバーが表示される場合は下記も同時に作成しておきましょう。
sidebar.php


ーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーー
２．style.cssの説明
ーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーー
/*
Theme Name: テーマ名
Theme URI: テーマのURL
Author: 作成者名
Author URI: 作成者のURL
Description: 説明書き
Version: バージョンの数値を書く
Text Domain: 言語ファイルで使う名称（必要なければ消しても構わない）
*/






ーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーー
２．header.phpの説明
ーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーー

//言語属性を付与
//出力結果：<html lang="jp">
//WordPressの「設定」＞「一般」＞「サイトの言語」から変更できます。
//参考URL：https://web-tsuku.life/language-attributes/

<html <?php language_attributes(); ?>>


//スマートフォンをはじめとしたモバイル端末でホームページを表示することを想定するとき、Viewportと呼ばれるタグを挿入します。
//参考URL：https://ferret-plus.com/6033

<meta name="viewport" content="width=device-width, initial-scale=1">


//使用されている文字コードを表示します（Version 3.5.0 以降は "UTF-8" を常に返します）。
//出力結果：<meta charset="UTF-8">
//参考URL：https://www.webdesignleaves.com/pr/wp/wp_func_geninfo.html

<meta charset="<?php bloginfo( 'charset' ); ?>">


