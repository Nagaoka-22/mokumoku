# README

## 環境構築
```
$ bundle install --without=production
$ bin/rails db:setup
$ yarn install
$ bin/webpack
$ bin/rails s
```

## 事業をエンジニアリングしよう提案編の回答は以下に記述してください

### 選択した事業側の課題
サービス登録者数の内、男性60%に対して、女性は40%。一方で、サービス内のもくもく会に参加した人の比率は、男性90%：女性10%と大きな差が出ています。もっと女性が使いやすいようなサービス設計にする必要があるのではないか？

### 提案内容
女性（男性）だけのもくもく会を作成できるようにする
→ 参加してみたら男10女1ような状態になることに抵抗を感じて参加していないのではないかと考えられる。

### 実装方針
* 会員情報に性別の項目を追加する。
* イベント作成時、女子（男子）会・指定なしを選べるようにする。
* 女子（男子）会は、女性（男性）会員にのみ表示および参加ができるようにする。
* 性別指定なしのイベントも「参加者」の欄で参加者の性別が表示されるようにする。