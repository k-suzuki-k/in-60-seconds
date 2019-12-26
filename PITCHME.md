### ポートフォリオ発表

---
### 何を作ったか？ 
![IMAGE](assets/img/presentation.png)

---
calcal(カルカル)という<br>
カレンダーを使った<br>
シンプルなtodo管理アプリを作成しました。<br>
<br>
名前の由来
-  Linuxでカレンダーを表示するコマンド`cal`
-  軽(カル)い気持ちで使って欲しい

---
###  題材を選んだ理由は？ 
![IMAGE](assets/img/presentation.png)

---
「こんなアプリを作りたい！！」というよりも、<br>
1～2か月の学習を通して感じた技術的な課題を<br>
克服できるようなポートフォリオを作成したかった。<br>
<br>
個人的な課題
-  javascriptの知識不足
-  viewを書くのが遅くてきれいでない
-  非同期処理の実装をしたことがない
-  テストコードの書き方がわからない
---
題材の方針は決まった
-  javascriptを積極的に使って、
できる限り画面推移させないように
非同期処理を実装する。
-  viewの効率的な書き方を学び実践する。
-  テストコードを書く時間を十分に設ける。

---
####  具体的に何を作るか？
→ 作りたいものが思いつかない<br>
<br>
→ googleカレンダーが便利だけど<br>
個人的に好きじゃないことを思い出す<br>
<br>
→ 決めた方針をもとに<br>
カレンダー使ったtodo管理アプリを作ろう

---
###  動作デモ
![IMAGE](assets/img/presentation.png)

---
###  工夫した点、苦労した点
![IMAGE](assets/img/presentation.png)

---
#### 課題:viewを書くのが遅くてきれいでない
-  **slim**を導入したことで記述量が激減した。  
-  読みやすくリファクタリングもしやすくなったので学習してよかった。  
-  helperを使えばもっとviewをきれいにできた。
```
= form_with(model: @user, local: true, class: "validate_field") do |form|
  .form-group
    = form.label :name, 'ユーザー名'
    = form.text_field :name, class: 'form-control validate[maxSize[20]]'

  .form-group
    = form.label :email, 'メールアドレス'
    = form.text_field :email, class: 'form-control validate[required,custom[email]] email_auto'
```
---
####  課題:非同期処理の実装をしたことがない
-  **jquery**やrailsの**js.erb**を用いて実装をした。  
-  非同期処理のおおまかな考え方・実装方法は  
身に着けたので細かい処理を覚える必要がある。  

---
####  課題:テストコードの書き方がわからない
-  Rspecの設定やテストデータの作り方(factory_bot)など
テストコード書くまでに時間が掛かった。
-  Rspecでテストできていない処理も多い。
-  「何をテストするべきか？」の考え方を身に着ける必要性を感じた。

---
####  新たな課題
-  javascriptのコードが冗長で汚い。
-  メイン機能の使い方がわかりづらかった。  
ユーザの使いやすさを意識する必要がある。 
-  デプロイしてから発生した問題があったので、  
本番環境を意識した開発が必要だと感じた。
（javascriptが起動しない、タイムゾーンがUTCになっている等）

---
ご清聴ありがとうございました!
