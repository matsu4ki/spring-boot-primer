---
next: '/hello-world/'
---

# データベースクライアント

データベースに接続してテーブルの情報や SQL の実行結果を見やすく整形して表示してくれる GUI アプリケーションを「データベースクライアント」ソフトと呼びます。データベースを使用した Web アプリケーションの開発では必須のアイテムですので、使い方を覚えておきましょう。

有料、フリー合わせて様々なデータベースクライアントソフトが存在しますが、Windows 環境であれば「A5:SQL Mk-2」がオススメです。

## データベースの作成

まずは今回のチュートリアルで使用するデータベースを作成しておきましょう。

```sql
CREATE DATABASE spring-demo;
```

## A5:SQL Mk-2 をインストールする

[こちらのページ](https://a5m2.mmatsubara.com/)の「Download !!」ボタンからダウンロードしてください。

![A5:SQL Mk-2](../assets/a5sqlmk2-homepage.png)

ダウンロードした zip ファイルを解凍して ```A5M2.exe``` をダブルクリックすると A5:SQL Mk-2 が起動します。

## データベースに接続する

メニュー「データベース」→「データベースの追加と削除」→「追加」→「PostgreSQL（直接接続）」と進むと以下の設定ダイアログが表示されます。

![A5:SQL Mk-2 設定ダイアログ](../assets/a5sqlmk2-setting.png)

* 「サーバー名」と「ポート番号」はそのままで OK です。
* 「データベース名」には先ほど作成した「spring-demo」を入力します。
* 「ユーザーID」と「パスワード」は各自で設定した値を入力します。

「テスト接続」をクリックしてエラーがなく正しく接続できていれば「OK」をクリックして設定を完了しましょう。
