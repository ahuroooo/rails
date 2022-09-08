# Ruby on Rails

## Ruby入門
https://www.javadrive.jp/ruby/

- Rubyインストールと環境設定～メソッド　まで実施しRuby基礎を理解


## Rails入門
https://www.javadrive.jp/rails/

- Ruby on Rails インストール～テンプレート(ビュー)とヘルパーメソッド　まで実施
- MYSQLへの接続 はスキップで（SQLiteのみできればOK）
- rakeコマンドはrailsコマンドへ置き換えてください
- Railsのversionの問題で手順通り進めるとcontlollerを生成する際にエラーとなることがあります。その際は下記を参考にGemfileを書き換えてください。

https://manabu-ito.hatenablog.com/entry/2021/08/31/162009

-------
## 課題（理解度チェック用）
GitHubに「Rails」という名前で公開リポジトリを作成してください。

masterブランチを作成後、そこから課題毎に開発用ブランチを作成し、

課題内容を必要に応じてpushしていってください。

課題が完成したらmasterブランチに向けてpull requestを作成し、

Slackで連絡して下さい。


※GitHubについての参考サイト

https://qiita.com/Ken227/items/822851aaca0fd9b3cf72

https://techacademy.jp/magazine/6235

ブランチの命名規則について

https://qiita.com/c6tower/items/fe2aa4ecb78bef69928f

## FizzBuzz問題
以下の仕様を満たすように、Rubyファイルを作成してください。

**仕様**
1から100までの連続した整数を画面に表示していく。ただし、
- もし、その整数が3で割り切れる数なら "Fizz" と表示する。
- もし、その整数が5で割り切れる数なら "Buzz" と表示する。
- 上記2つの条件は同時に満たせる。つまり、もし、その整数が3で割り切れ、なおかつ5で割り切れる数なら "FizzBuzz" と表示する。
- それ以外の数は、その数をそのまま表示する。


-------
## ピタゴラス（三平方の定理）プログラムを作ろう
三平方の定理は、直角三角形の3つの辺について、直角をはさむ2つの辺の長さをそれぞれ a と b、斜辺の長さを c としたとき、以下のような関係が成り立つという公式です。

`cの二乗 = aの二乗 + bの二乗`

以下の仕様を満たすように、ファイルを作成してください

- WebサーバはSinatraで立てる事
- GETパラメータを2つ使用（aとb）
- 2つの辺の長さを取得し、三平方の定理を使って cの二乗 を求める
- 平方根のcを求め、以下のように画面に表示する
```
直角をはさむ2辺の長さが 3.0 と 4.0 のとき、 斜辺の長さは 5.0 になります。
```

Sinatraについての参考

https://dev.classmethod.jp/articles/sinatra__make_api_server/

-------
### タスク管理アプリケーションを作ろう
以下の仕様を満たすように、Webアプリケーションを作成してください

- scaffoldは使用しない
- DBはSQlite使用
- formについてはrailsのform withを使用
　https://pikawaka.com/rails/form_with
- strong parameterを使用
　https://qiita.com/ozackiee/items/f100fd51f4839b3fdca8

- タスクを保存するtasksテーブルを作成する。カラムは以下４つ。
  - ID
  - タスクの内容
  - 作成日時
  - 更新日時
<br><br>
- タスクに対する以下7つのアクションをすべて実装してください

　このシステムではリソース＝タスクのことになります

| アクション | 概要 | HTTPメソッド |
| -------- | -------- | -------- |
|index |登録済みのリソースを一覧表示する画面 |GET|
|show |リソースの詳細な情報を表示する画面 |GET|
|new |新しいリソースの入力画面（フォーム） |GET|
|create |新規登録処理（INSERT） |POST|
|edit |既存のリソースの編集画面（フォーム） |GET|
|update |変更処理（UPDATE） |PATCH|
|destroy |削除処理（DELETE） |DELETE|

<br>
※これらのアクションはREST（REpresentational State Transfer）の概念で定義されています。
RESTについての参考ページ
https://www.javadrive.jp/rails/routing/index5.html#section1

<br>

- 画面は、以下４つが必要になります
  - index（タスク一覧）
  - show（詳細ページ）
  - new（作成ページ）
  - edit（編集ページ）




