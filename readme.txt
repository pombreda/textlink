========================================================================
           テキストリンク for Netscape 7 & Mozilla & Firefox
========================================================================
[名称       ] テキストリンク for Netscape 7 & Mozilla & Firefox
[バージョン ] 1.3.2006100702
[種別       ] フリーソフトウェア
[制作者     ] Piro(下田 洋志)
[最終更新   ] 2006/10/7
[圧縮形式   ] LHA
[動作環境   ] Netscape 7.0 以上あるいはMozilla 1.0 以上が動作する環境。
              当方ではWindows2000上で、Mozilla Firefox 2.0 RC2 にて動作
              の確認を行っています。

[転載/再配布] 無断転載・再配布は自由に行っていただいて構いません。改造し
              たものを公開することも制限しません。ただしクレジットは元の
              ものを残すようにしてください。
              このパッケージに含まれるコードの殆どは MPL 1.1, GPL 2.0,
              および LGPL 2.1 のトリプルライセンスとなっていますので、
              これらの点については、それぞれのライセンスの条件に従って下
              さい。
              なお、書籍の付録CD-ROMやソフトウェア等へ収録していただける
              場合は、必ず事前にご連絡下さい。

[著作権     ] このパッケージに含まれるプログラムの著作権はPiro(下田 洋
              志)が保有します。多分。
              ていうかプログラムに著作権って認められるんだっけ？ しかも
              UIはXMLだし。文書インスタンスのマークアップに著作権は発生
              しないというのが公の見解だったような気も……

[連絡先     ] piro.outsider.reflex@gmail.com
[配布元     ] http://piro.sakura.ne.jp/
              http://hp.vector.co.jp/authors/VA016061/


========================================================================
＊目次

  ・ヘッダ
  ・目次
  ・ファイル構成
  ・紹介
  ・インストール手順
  ・アンインストール手順
  ・免責
  ・更新履歴（抜粋）


========================================================================
＊ファイル構成

  ・readme.txt   : 取扱説明(このファイル)
  ・textlink.xpi : XPInstall Package本体

 ※どちらも、インストール後は削除してかまいません。


========================================================================
＊紹介

ページ中に書かれたURI文字列を、ダブルクリックするだけでリンクのように
開けるようにします。


========================================================================
＊インストール手順

  +-----------------------------------------------------------------+
  | ※旧バージョンからの更新の場合、インストールを始める前に、必    |
  |   ず、次項の「アンインストール手順」に従って旧バージョンをア    |
  |   ンインストールしておいて下さい。旧バージョンのファイルが残っ  |
  |   ている場合、導入に失敗したり、NS/Mozの動作に支障が出る場合    |
  |   があります。                                                  |
  | ※インストールを行う前に、Preferences（設定） >                 |
  |   Advanced（詳細） > Software Installation（ソフトウェアのイ    |
  |   ンストール）で「Enable software installation（ソフトウェア    |
  |   のインストールを可能にする）」にチェックを入れて下さい。      |
  | ※Mozilla 1.3以前では、管理者権限でないとインストールできませ   |
  |   ん。導入は必ず、rootあるいはadminでログオンして行って下さい。 |
  +-----------------------------------------------------------------+

step1: ファイルのコピー
  textlink.xpiをブラウザのウィンドウにドロップすると、インストール
  が開始されます。
  途中、日本語の言語パックを登録するかどうかの確認があるので、必要に応じ
  て選択して下さい。

step2: NS/Mozの再起動
  ファイルのコピーが終わったら、NS/Mozを再起動します。
  コピーしたファイル群が、起動時にNS/Mozに登録されます。


========================================================================
＊アンインストールの手順

Preferences（設定） > Advanced（詳細） > Text Link（テキストリンク）で
「Uninstall（アンインストール）」と書かれたボタンをクリックすると、
自動でアンインストールが行われます。

なお、ファイルの削除は自動では行われません。表示されるメッセージに従っ
て、ブラウザを終了させた後に、指定されたファイルを手動で削除して下さい。


ブラウザ自体起動できないなどの緊急の場合には、以下の手順に従って、手動で
アンインストールを行って下さい。

  1. NS/Moz を終了させる。簡易起動（高速起動）が有効になっている場合、
     タスクトレイのアイコンを右クリックして、そちらも終了させる。
  2. ユーザープロファイルディレクトリか、 NS/Moz をインストールした
     ディレクトリ（管理者権限でインストールした場合）の中にある
     /chrome/ フォルダから、 textlink.jar, overlayinfo ディレクトリ,
     chrome.rdf を削除する。
  3. 管理者権限でインストールした場合、installed-chrome.txt をメモ帳等
     で開き、以下の行を削除する。
     ・content,install,url,jar:resource:/chrome/textlink.jar!
                           /content/textlink/
     ・locale,install,url,jar:resource:/chrome/textlink.jar!
                           /locale/en-US/textlink/
    (・locale,install,url,jar:resource:/chrome/textlink.jar!
                           /locale/ja-JP/textlink/)

この手順では設定情報などが残ったままになりますが、ブラウザを使用する上
では問題ありません。


========================================================================
＊免責

このパッケージを使用した事により発生したいかなる障害に対しても、制作者
は一切の責任を持ちません。全て使用者の個人の責任に基づくものとします。


========================================================================
＊更新履歴（抜粋）

1.3.2006100702
    ・Firefox 2.0 の大量のタブを開く前の警告に対応
1.3.2006100701
    ・Firefox 2.0 のタブのオーナー機能に対応
1.3.2006032801
    ・フランス語の言語パックを修正（by menet）
1.3.2006032701
    ・URI文字列を選択するのみの「選択モード」を加えた
    ・URI文字列を選択する時、前後の余計な文字列まで選択されたま
      まになってしまうことがあったのを修正
1.3.2006032601
    ・Find As You TypeでURI文字列の一部が選択された状態やキャ
      レットブラウズモードでURI文字列の中にカーソルがある場合に
      おいて、EnterキーでURI文字列を読み込めるようにした
    ・相対パスの解釈を有効にしているとき、コンテキストメニュー
      の項目の初期化に失敗することがあったのを修正
1.3.2006031401
    ・選択範囲のURI文字列をコンテキストメニューから開く場合、部
      分選択されたURIも常に含めるようにした
    ・相対パスの解釈を有効にしているとき、スペースを空けてURI文
      字列の前に書かれた語句までURIの一部と見なすことがあった問
      題を修正
    ・フランス語の言語パックを同梱した（made by menet）
1.3.2006031301
    ・動作モードの設定を正しく保存・読み込みできなくなっていたの
      を修正
    ・相対パスと全角文字の解釈を同時に有効にするとURIの検出に失
      敗することがあったのを修正
    ・タブを開く設定の時、常に全面のタブで開かれていたのを修正
1.3.2006031201
    ・補完するパターンにワイルドカード（*、?）を使えるようにした
    ・括弧を含むURIの認識精度を少し改善
    ・スキーマを省略されて「www」などから始まるURI文字列も補完で
      きるようにした
    ・全角文字を半角文字に置換する処理のアルゴリズムを高速化した
      （based on implementation written by Taken,
      http://taken.s101.xrea.com/blog/article.php?id=510）
    ・設定パネルの構成を変更
    ・デフォルトの設定を変更
1.3.2006031001
    ・英語の言語パックのミスを修正
    ・複数のURI文字列を選択したときのコンテキストメニュー項目の
      ラベルがおかしくなっていたのを修正
    ・「h**p」「h++p」などの形でエスケープ（？）されたURI文字列
      も解釈できるようにした
    ・解釈するスキーマなどの設定を、カンマ以外の文字でも区切れる
      ようにした
1.3.2006030901
    ・単純なダブルクリックだけではなく、Ctrlキーなどとの組み合わ
      せもトリガーとして設定できるようにした
    ・新しいタブをフォアグラウンドで開くかバックグラウンドで開く
      かに関する設定の実装方法を変えた
    ・長いページでコンテキストメニューの展開やクリック位置の検出
      に時間がかかる問題を修正
    ・隠し設定でURI検索範囲の大きさを指定できるようにした
      （textlink.find_range_size）
1.3.2006022101
    ・右クリック時のコンテキストメニューの内容を少し変更
1.3.2005121301
    ・クリック位置の検出を緩く判定するようにすると、却って判定が
      厳しくなってしまっていたのを修正
1.3.2005070402
    ・クリックしたURI文字列を読み込めない問題を修正
    ・ダブルクリックでURI文字列をタブで開いたときに、URI文字列を
      選択するようにした
1.3.2005070401
    ・クリックしたURI文字列を読み込めないケースがあったのを修正
1.3.2005062901
    ・一部のページでクリックしたURI文字列を読み込めないことがあった
      のを修正
1.3.2005062801
    ・XUL/Migemoを参考に、URI文字列が複数のノードに分割されていても
      一続きのURI文字列として認識できるようにした

------------------------------------------------------------------------
Text Link for NS7 & Moz & Firefox
Copyright 2004-2006 Piro(YUKI "Piro" Hiroshi)
