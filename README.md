# Procom 蔵書検索
https://nit-maizuru-programmers-community.github.io/ProcomOPAC/

## 概要

舞鶴高専プロコン部の蔵書データを検索・閲覧できるサイトです。キーワードや詳細条件で本を検索し、一覧や詳細を表示できます。

## ファイル構成

- index.html：トップページ・検索画面
- books.html：蔵書一覧ページ
- result.html：検索結果表示ページ
- img/NoImage.png：書影がない場合の画像

## 蔵書データ
プロコン部のGDrive>Web_Site>ProcomOPAC(フォルダ)>ProcomOPAC(ファイル)から編集ができます。（学校アカウント必須）

可能であればデータ追加後、「範囲を並べ替え」▶「列Aを基準に昇順で範囲を並べ替え」でデータを整理してもらえるとありがたい。

データ配列
- title：本のタイトル(A)
- author：本の著者(B) いなければ空欄でも可
- publisher：発行者(C)
- isbn：ISBN(D)
- img：画像アドレス(E) なければ空欄でも可

データはAppsScriptを使用して取ってきている。変更があれば「デプロイ▼」▶「新しいデプロイ」から、

- 種類の選択：ウェブアプリ
- 説明：デプロイの説明
- 次のユーザーとして実行：自分
- アクセスできるユーザー：全員

で、デプロイ。

表示されたウェブアプリのURLをコピーしてindex.htmlのbooksApiUrlに貼り付けして終わり。