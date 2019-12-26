### ポートフォリオ発表
id:k-suzuki-k

---
### 自己紹介
![IMAGE](assets/img/presentation.png)
---
-  茨城県出身
-  27歳
-  趣味
	-  読書(人文系)
	-  ギター
	-  スヌーピー
	-  vim

---
### 何を作ったか？ 
![IMAGE](assets/img/presentation.png)

---
calcal(カルカル)という名前の<br>
カレンダーを使ったシンプルな<br>
todo管理アプリを作成しました。<br>
<br>
名前の由来
-  Linuxでカレンダーを表示するコマンド`cal`
-  軽(カル)い気持ちで使って欲しい
-  HUNTER×HUNTERが好き

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
-  viewを書くのが遅くて汚い
-  非同期処理の実装をしたことがない
-  テストコードの書き方がわからない

---
題材の方針は決まった
-  javascriptを積極的に使って、<br>
できる限り画面推移させないように<br>
非同期処理を実装する。
-  viewの効率的な書き方を学び実践する。
-  テストコードを書く時間を十分に設ける。

---
####  具体的に何を作るか？
→ 作りたいものが思いつかない、、<br>
→ googleカレンダーが便利だけど個人的に好きじゃないことを思い出す<br>
→ 決めた方針をもとにカレンダー使ったtodo管理を作ろう

---
###  動作デモ
![IMAGE](assets/img/presentation.png)
---
###  工夫した点、苦労した点
![IMAGE](assets/img/presentation.png)
---
#### 課題:viewを書くのが遅くて汚い

slimを導入したことで記述量が激減した。  
読みやすくリファクタリングもしやすくなったので、  
学習してよかった。
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
