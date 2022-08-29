# slack-api-db2

## NodeJSとSlack APIによるいまどきのネットワークプログラミング

### データベースにアクセスする その2

Slackからデータベースに接続して、その内容を画面に反映する。そのため、データベースの基本操作とNode.jsから接続する方法を学ぶ。ここではモーダルビューを通してデータベースに注釈（コメント）を登録する方法を習得する。

[動作確認の手順]

1. コマンドプロンプトを開き、ダウンロードしたフォルダへ移動する
1. npm installコマンドでアプリに依存するパッケージをインストールする
1. .envファイルの環境変数SLACK_BOT_TOKEN、SLACK_APP_TOKEN、DB_URLが正しく設定されているか確認する
1. アプリを起動する
    $ node ./app.js
1. Slackアプリをインストールしたチャネルのメッセージ欄に「/covid19」と入力し、送信する
1. 選択メニューから適当な国を選ぶ
1. 感染状況の下に[コメント]ボタンが配置されていることを確認する
1. このボタンをクリックすると該当国へのコメント入力モーダルビューが現れる
1. コメントを記入し、登録ボタンをクリックする（登録されたと返答がある）
1. [再表示]ボタンをクリックすると、コメントを入力した日時と内容が感染状況の下に現れることを確認する
