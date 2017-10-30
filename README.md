要約 プログラマが知るべき97のこと＋１０ 
by Kevlin Henney 和田卓人、夏目大

- [O'Reilly Japan - プログラマが知るべき97のこと](
https://www.oreilly.co.jp/books/9784873114798/)

- [97 Things Every Programmer Should Know - O'Reilly Media](http://shop.oreilly.com/product/9780596809492.do)

- [97 Things Every Programmer Should Know - Programmer 97-things](http://programmer.97things.oreilly.com/wiki/index.php/97_Things_Every_Programmer_Should_Know)


# 1. [分別のある行動](https://プログラマが知るべき97のこと.com/エッセイ/分別のある行動)

[ (英文=> by Seb Rose)](http://programmer.97things.oreilly.com/wiki/index.php/Act_with_Prudence)
技術的負債
故意による技術的負債と不注意から発生する技術的負債がある。
この２つは区別すべき。
この技術的負債の存在は常に忘れないようにし、できるだけ早く返済すべきです。

- http://martinfowler.com/bliki/TechnicalDebt.html
- http://martinfowler.com/bliki/TechnicalDebtQuadrant.html


# 2. [関数型プログラミングを学ぶことの重要性](https://プログラマが知るべき97のこと.com/エッセイ/関数型プログラミングを学ぶことの重要性)

[ (英文=> by Edward Garson)](http://programmer.97things.oreilly.com/wiki/index.php/Apply_Functional_Programming_Principles)
関数型プログラミングのパラダイムを十分に学べば、その知識、技術はマルチコアへ
の対応以外にも幅広く役立つでしょう。
重要なのは参照透過性が向上するということです。
これは関数がどこでいつ呼び出されようと、入力が同じであれば、常に得られる結果が
同じになるということを意味します。
大事なことは可変なメンバー変数の参照が必要になるような設計をしないことです。
それよりも小さな関数を数多く作り、個々の役割を限定するほうが得策です。

- http://www.jmock.org/oopsla2004.pdf

# 3. [ユーザが何をするかを観察する（あなたはユーザではない）](https://プログラマが知るべき97のこと.com/エッセイ/ユーザが何をするかを観察する-あなたはユーザではない)

[ (英文=> by Giles Colborne)](http://programmer.97things.oreilly.com/wiki/index.php/Ask_%22What_Would_the_User_Do%3F%22_%28You_Are_not_the_User%29)
誰もが自分と同じような物の見方や考え方をするはずだと思いこむ、
こういった誤った思い込みのことを心理学用語で偽の行為効果といいます。
実際には人によって物の見方や考え方は大きく違います。
ユーザーの行動を知るにはどうすればいいか？ユーザーを観察するのが一番です。
実は、ユーザーが求めているものを正しく知るには、言葉を聞くよりも彼らの行動を観察するほうがいいのです。
彼らの求めるものを頭で考えて１日過ごすよりも、わずか１時間でも観察をしたほうが
得るものは多いでしょう。

- https://ja.wikipedia.org/wiki/偽の合意効果

# 4. [コーディング規約を自動化する](https://プログラマが知るべき97のこと.com/エッセイ/コーディング規約を自動化する)

[ (英文=> by Filip van Laenen)](http://programmer.97things.oreilly.com/wiki/index.php/Automate_Your_Coding_Standard)
コーディング規約は可能な限り、自動的、かつ強制的に守られるようにすべきでしょう。
* コードの整形処理をビルドプロセスに含めてしまう
* 静的なコード解析ツールを使用して望ましくないアンチパターンがないか探す。
* ツールの設定により、プロジェクト固有のアンチパターンも見つけ出せるようにする。
* テストカバレッジをただ計測するだけで終わらせるのではなく、
計測結果の判定も自動的に行われるようにする。
基本的に、自分を含めチームの人達は規約を忠実に守らないと考えておくべきでしょう。
もう一つ大切なことは、コーティング規約は常に変化していくべきということです。

# 5. [美はシンプルさに宿る](https://プログラマが知るべき97のこと.com/エッセイ/美はシンプルさに宿る)

[ (英文=> by Jørn Ølmheim)](http://programmer.97things.oreilly.com/wiki/index.php/Beauty_Is_in_Simplicity)
ソフトウェア開発者ならば常に心に留めておくべき言葉
「文章にしろ、和音にしろ、リズムにしろ、美しく、優雅なもの、優れたものはすべてシンプルである」
ｂｙプラトン
プログラマーがコードを書く時に留意すべきこと
* 可読性
* 保守性
* 開発効率
* （言葉で表現するのが難しい）美しさ

今まで見てきた優れたコードの中で幾つかの共通の特徴がありました。
その中でも特に重要なのが「シンプルである」ということです。
システム全体がどれだけ複雑であろうと、個々で見れば全てシンプルになっています。

# 6. [リファクタリングの際に注意すべきこと](https://プログラマが知るべき97のこと.com/エッセイ/リファクタリングの際に注意すべきこと)

[ (英文=> by Rajith Attapattu)](http://programmer.97things.oreilly.com/wiki/index.php/Before_You_Refactor)
リファクタリングの時注意すべきこと。
* リファクタリングをするにあたってはじめにすべきことは、
既存のコードベースと、そのコードに対して書かれたテストコードを洗い直す。
* すべてをゼロから書き直したい衝動にかられることもありますが、
その誘惑に打ち勝たなければなりません。
* 一度に大きな変更を加えるよりも、少しずつの変更を数多くすべきです。
* 各イテレーションの最後には、既存のテストが通るか必ず確認します。
* 個人の好みやエゴをいれてはなりません。
* 新技術を使いたい、というのもそれだけではリファクタリングの十分な理由にはなりません。
* 人間は必ずミスをする、ということを常に忘れないようにしましょう。

# 7. [共有は慎重に](https://プログラマが知るべき97のこと.com/エッセイ/共有は慎重に)

[ (英文=> by Udi Dahan)](http://programmer.97things.oreilly.com/wiki/index.php/Beware_the_Share)
再利用する時に「コンテキスト」を気をつける。
「再利用」は一般的には良いこととされており、たしかに基本的には良いことです。
しかし、コンテキストが不適切だと、メリットよりもコストのほうが大きくなるのです。

# 8. [ボーイスカウト・ルール](https://プログラマが知るべき97のこと.com/エッセイ/ボーイスカウト-ルール)

[ (英文=> by Uncle Bob)](http://programmer.97things.oreilly.com/wiki/index.php/The_Boy_Scout_Rule)
「モジュールをチェックインする際には、必ずチェックアウト時よりも美しくする」
どこか一箇所でいいので改善しましょう
変数名をより適切なものに変えたり、
大きい関数を2つの小さくよりシンプルな関数に分割する
循環関数を解消するというのもいいですし
インターフェースを追加することで、ポリシーと実装を切り離すというのでもいいでしょう。

# 9. [他人よりまず自分を疑う](https://プログラマが知るべき97のこと.com/エッセイ/他人よりまず自分を疑う)

[ (英文=> by Allan Kelly)](http://programmer.97things.oreilly.com/wiki/index.php/Check_Your_Code_First_before_Looking_to_Blame_Others)
何か問題が起きた時には、まず真っ先に自分の書いたコードを疑います。
自分のコードを徹底的に調べ、それでもバグが見つからないならば
コンパイラのバグを疑い、スタック汚染を調査します。


- [シャーロック・ホームズ―世界の名探偵コレクション10〈1〉 (集英社文庫) 文庫](http://amzn.to/2i1uTD7)

- http://en.wikipedia.org/wiki/Dirk_Gently

# 10. [ツールの選択は慎重に](https://プログラマが知るべき97のこと.com/エッセイ/ツールの選択は慎重に)

[ (英文=> by Giovanni Asproni)](http://programmer.97things.oreilly.com/wiki/index.php/Choose_Your_Tools_with_Care)
まずは最低限のツールだけを導入する。
よく検討して、どうしても必要と判断したものだけに絞り込んで導入するのです。
このアプローチによって、当初の予測よりも導入するツールが少なくて済み、
アプリケーションも肥大せずにすむのです。

- [検索：GPL 誤解](https://www.google.co.jp/search?q=GPL+誤解)

# 11. [ドメインの言葉を使ったコード](https://プログラマが知るべき97のこと.com/エッセイ/ドメインの言葉を使ったコード)

[ (英文=> by Dan North)](http://programmer.97things.oreilly.com/wiki/index.php/Code_in_the_Language_of_the_Domain)
コードがどの概念を表現しているのかは、出来る限りひと目で分かるようにしておくべきです。
何ヶ月か時間が立ってからコードを見たプログラマは、きっと最初にコードを
書いた人に感謝するでしょう、そしてそのプログラマは、最初にコードを書いた
本人かもしれないのです。

# 12. [コードは設計である](https://プログラマが知るべき97のこと.com/エッセイ/コードは設計である)

[ (英文=> by Ryan Brush)](http://programmer.97things.oreilly.com/wiki/index.php/Code_Is_Design)
「コードを書くことは設計をすることである」
機械的な作業ではなく、創造的な仕事なのだと。
ソフトウェア開発がなぜ今、危機に陥っているのか
何より危機に陥っているのは設計です
作る人間の能力を超える程の高度な製品、複雑な設計を求められていて、
しかも、製品を早く市場に出せという圧力が強いような状況では、
設計が不十分なまま製品が作られることがどうしても多くなるのです。
どうすればよいか？
「自動テスト」
多数の過酷なテストに耐えるものであると証明されない限り、
設計が完了したとはみなさないようにするのです。
決して忘れてならないのは、優れた設計には優れた設計のできる「人間」が要る、
ということです。そういう人間になるためには、技術の取得のため相当の努力が
必要になります、コーディング能力も例外ではありません。

# 13. [コードレイアウトの重要性](https://プログラマが知るべき97のこと.com/エッセイ/コードレイアウトの重要性)

[ (英文=> by Steve Freeman)](http://programmer.97things.oreilly.com/wiki/index.php/Code_Layout_Matters)
プログラマの仕事はコードを書く時間よりも、コードを探すことと読むことに費やしている。
と言う調査結果もあるようです。
そこで、私はなんとかこの「探したり、読んだり」の効率化を図りたいと考えました。
* 目立たない部分を作る
ドメインに直接関係のない部分を他の部分より目立たせないようにする
人間の視覚は他と違っている場所をすぐ見つけられるように出来ているのです。
* レイアウトに語らせる
コードを構成する各部分はどんな役割を持っているかすぐ分かる名前をつけるべき
また名前だけでなく、見てすぐ分かるコードを書くためにはレイアウトも重要です。
* コンパクトにまとめる
現在はディスプレイの制約のほうが大きいのです、画面に一度に表示できるものが
多くなれば、スクロール量やファイルの切り替えが少なくてすみます。
つまり「コンテキストが分断される」ことが減るわけです。
できるだけ多くの要素を一度に見せたほうが、コードは理解しやすくなります。
私は本当に素晴らしいコードを見たときは詩みたいに感じたことがありました
書かれた文字が全て何かしらの目的を持っていて、しかも見るだけでその目的が
度言う言うものなのかすぐに分かる、そんなコードでした。

# 14. [コードレビュー](https://プログラマが知るべき97のこと.com/エッセイ/コードレビュー)

[ (英文=> by Mattias Karlsson)](http://programmer.97things.oreilly.com/wiki/index.php/Code_Reviews)
コードの質を上げ、欠陥を減らす
チーム全員に同じ知識を共有させること、
コーディングにおいて全員が守るべきガイドラインを確立すること
レビューは建設的であること、辛辣な批判はしない
そして、楽しくレビューすること。

# 15. [コードの論理的検証](https://プログラマが知るべき97のこと.com/エッセイ/コードの論理的検証)

[ (英文=> by Yechiel Kimchi)](http://programmer.97things.oreilly.com/wiki/index.php/Coding_with_Reason)
生きたオブジェクトの値を簡単に説明できるようにしておく。
gotoは避ける
変更可能なグローバル変数は使わない
変数のスコープは出来る限り小さく、最初に使用する場所で宣言する
オブジェクトは可能な限り不変immutableにする
縦横にスペースを入れて見やすくする。
オブジェクト、型、関数にできるだけわかりやすく、短い名前をつける
セクションを入れ子にする必要が出たときは関数にする。
関数は短く、機能を一つに絞る 24行制限 1画面に収まる程度
関数のパラメーターはできるだけ少なく、多くても4つまで
インターフェースはできるだけ短くする。 カプセル化
クラスでsetterの使用は推奨できない

# 16. [コメントについてのコメント](https://プログラマが知るべき97のこと.com/エッセイ/コメントについてのコメント)

[ (英文=> by Cal Evans)](http://programmer.97things.oreilly.com/wiki/index.php/A_Comment_on_Comments)
コメントを書く、コードは次に見る人がすぐに理解できるように書く
格言「書くのに苦労したコードは、読むのにも苦労する」
ヘッダコメントに、プログラマがコード本体を全く読まなくても利用することは出来るぐらいのコメントを書く
インラインコメントには、自分の次にコードを見て修正、拡張する人の助けになるような情報を盛り込む

# 17. [コードに書けないことのみをコメントにする](https://プログラマが知るべき97のこと.com/エッセイ/コードに書けないことのみをコメントにする)

[ (英文=> by Kevlin Henney)](http://programmer.97things.oreilly.com/wiki/index.php/Comment_Only_What_the_Code_Cannot_Say)
良いコメントを書くための文章術
コメントに書かなくても良いことを見極める技術
読む人にとって価値があるコメントとは
コードには書いてないことや、コードには書けないことが書いてあるコメント
メソッド名やクラス名がわかりにくかったら名前を変える、
関数が長くてコメントを書いているなら関数を小さく分割する
コード自身に語らせる
それが不可能な時、語らせたかったものとコードとのギャップをこそコメントに書く
コードに「書いていないこと」では無く、「コードに書けないこと」のみをコメントにする

- [プログラム書法-第2版-Brian-W-Kernighan](http://amzn.to/2gzPlL2)

# 18. [学び続ける姿勢](https://プログラマが知るべき97のこと.com/エッセイ/学び続ける姿勢)

[ (英文=> by Clint Shank)](http://programmer.97things.oreilly.com/wiki/index.php/Continuous_Learning)
具体的には
雑誌、書籍、ネット、slackに参加
本当に身につけたい技術は、コードを自ら書き、手を動かして学ぶ。
自分より上のレベルの人と仕事をする
自分の良き師をネットで探し、勉強になると感じればその人のブロブなどをチェック
自分が利用しているフレームワーク、ライブラリのソースを見る
デバッガを使ってコードを逐一確認する
ミスをした時、バグを修正した時、その問題について深く理解するよう務める
googleさえあれば、ほぼどんな情報でも見つかる。
自分が学んだことを誰かに教える
誰かが自分の話を聞き、質問してくると思えば学ぶ意欲は自然と高まる
勉強会に参加or立ち上げる
カンファレンスに参加、もしくはオンラインで動画やスライドなどを見る。
通勤時間を利用してポッドキャストを聞く
自分が書いたコードに静的分析ツールを実行する
IDEなどを使用していた場合、警告が出たらなぜその警告が出たのかを調べる
毎年一つは、新しい技術、言語、ツールのどれかに触ってみる
新しく学ぶものはコンピュータ関連でなくてもかまわない
生産性を高める方法なども学んで見る
学校に通う N予備校 udemy dotinstall
1週間に1回１時間でもいい、なにもしないよりまし。
技術はすごい勢いで進歩していき、
学ばなければおいていかれる。

- [新装版-達人プログラマー-職人から名匠への道-Andrew-Hunt](http://amzn.to/2z57ZpG)

- [Pragmatic-Programmer-Journeyman-Master](http://amzn.to/2z45S5i)


# 19. [誰にとっての「利便性」か](https://プログラマが知るべき97のこと.com/エッセイ/誰にとっての-利便性-か)

[ (英文=> by Gregor Hohpe)](http://programmer.97things.oreilly.com/wiki/index.php/Convenience_Is_not_an_-ility)
作る側にとっての便利さと、使う側にとっての便利さは違う。

# 20. [すばやくデプロイ、こまめにデプロイ](https://プログラマが知るべき97のこと.com/エッセイ/すばやくデプロイ-こまめにデプロイ)

[ (英文=> by Steve Berczuk)](http://programmer.97things.oreilly.com/wiki/index.php/Deploy_Early_and_Often)
インストールやデプロイの訓練に時間を割こう。軽視しがちである

# 21. [技術的例外とビジネス例外を明確に区別する](https://プログラマが知るべき97のこと.com/エッセイ/技術的例外とビジネス例外を明確に区別する)

[ (英文=> by Dan Bergh Johnsson)](http://programmer.97things.oreilly.com/wiki/index.php/Distinguish_Business_Exceptions_from_Technical)
例外処理は自分でコードを書かず、トップレベルの例外処理メカニズムに依頼する
具体的に、トランザクションのロールバック、ログ作成、管理者への警告、ユーザーへの通知など
ビジネス例外を技術的例外と一緒に扱わない
技術的例外とはそのエラーによってアプリケーションが動作不能になること
ビジネス例外とはユーザーが間違わないようにわざと警告を発生させる事
ユーザーが貯金額を超える金額を引き下ろそうとした時とか

# 22. [1万時間の訓練](https://プログラマが知るべき97のこと.com/エッセイ/1万時間の訓練)

[ (英文=> by Jon Jagger)](http://programmer.97things.oreilly.com/wiki/index.php/Do_Lots_of_Deliberate_Practice)
週に20時間なら10年、ゆっくりと成長していく。
訓練は楽にこなせない課題を選ぶこと
自分の能力を少し超える課題に取り組むことが重要だ
困難な課題に挑戦し、その結果を分析し、何か失敗すれば修正する、その繰り返しだ。

- http://norvig.com/21-days.html
- [リーンソフトウェア開発と組織改革-Mary-Poppendieck-依田光江-依田智夫](http://amzn.to/2zMxUzi)
- [Leading-Lean-Software-Development-Addison-Wesley-ebook](http://amzn.to/2zMIA17)

# 23. [ドメイン特化言語 DSL](https://プログラマが知るべき97のこと.com/エッセイ/ドメイン特化言語)

[ (英文=> by Michael Hunger)](http://programmer.97things.oreilly.com/wiki/index.php/Domain-Specific_Languages)
DSL ある分野に固有の語彙や語法を使用して事象を表現できるように作り上げられたプログラミング言語。
内部DSL、外部DSL

- [Art-UNIX-Programming-Eric-S-Raymond](http://amzn.to/2zMneRi)
- [UNIX-Programming-Addison-Wesley-Professional-Computing](http://amzn.to/2z4rz5b)
- [Domain-Specific-Languages-Addison-Wesley-Signature-Fowler](http://amzn.to/2zN2zfZ)

# 24. [変更を恐れない](https://プログラマが知るべき97のこと.com/エッセイ/変更を恐れない)

[ (英文=> by Mike Lewis)](http://programmer.97things.oreilly.com/wiki/index.php/Don%27t_Be_Afraid_to_Break_Things)
リファクタリングをしましょう。
リファクタリングは治療です、行えばチームがシステムを深く知ることが出来ます。
その投資は十分回収できるでしょうし、何倍もの利益となって返ってくるでしょう

- https://ja.wikipedia.org/wiki/ジェンガ
- [リファクタリング―既存のコードを安全に改善する―-OBJECT-TECHNOLOGY-Martin-Fowler](http://amzn.to/2gyKzxi)
- [Refactoring-Improving-Existing-Addison-Wesley-Technology-ebook](http://amzn.to/2gyUFOV)
- [レガシーコード改善ガイド-Object-Oriented-SELECTION-マイケル-C-フェザーズ](http://amzn.to/2hnk66J)
- [Working-Effectively-Legacy-Michael-Feathers](http://amzn.to/2gxYowe)
- [特別扱いする - 学校では教えてくれないバッドノウハウ英語 #9 - bkブログ](http://0xcc.net/blog/archives/000165.html)

# 25. [見られて恥ずかしいデータは使わないこと](https://プログラマが知るべき97のこと.com/エッセイ/見られて恥ずかしいデータは使わないこと)

[ (英文=> by Rod Begbie)](http://programmer.97things.oreilly.com/wiki/index.php/Don%27t_Be_Cute_with_Your_Test_Data)
例
進捗会議中「二度とクリックするんじゃねーぞ、バーカ」というメッセージが表示される。
あるプログラマが、レガシーシステムのエラーログの追加を指示される。
もともと裏で動いていたものだった。
保守作業によって「おい、バットマン、データベースの糞野郎がへましやがったぜ！」
というメッセージが画面に表示されユーザーから見られるようになった。

- [ティッカーシンボル - Wikipedia](https://ja.wikipedia.org/wiki/ティッカーシンボル)
- http://www.kuro5hin.org
- http://www.kuro5hin.org/story/2004/2/15/71552/7795

# 26. [言語だけでなく文化も学ぶ](https://プログラマが知るべき97のこと.com/エッセイ/言語だけでなく文化も学ぶ)

[ (英文=> by Anders Norås)](http://programmer.97things.oreilly.com/wiki/index.php/Don%27t_Just_Learn_the_Language%2C_Understand_its_Culture)
新しい言語から新たな発想を得て、同じ問題に対して違った解決策を
見つけられるようになるのが大事。
新たな言語を学べば、従来から使っていた言語でも、より美しいコードが
書けるようになることが多いのです。

- [新装版-達人プログラマー-職人から名匠への道-Andrew-Hunt](http://amzn.to/2z57ZpG)
- [Pragmatic-Programmer-Journeyman-Master](http://amzn.to/2z45S5i)
- [オブジェクト指向における再利用のためのデザインパターン-エリック-ガンマ](http://amzn.to/2i2SovC)
- [Design-Patterns-Object-Oriented-Addison-Wesley-Professional](http://amzn.to/2i1Lg2x)

# 27. [死ぬはずのプログラムを無理に生かしておいてはいけない](https://プログラマが知るべき97のこと.com/エッセイ/死ぬはずのプログラムを無理に生かしておいてはいけない)

[ (英文=> by Verity Stob)](http://programmer.97things.oreilly.com/wiki/index.php/Don%27t_Nail_Your_Program_into_the_Upright_Position)
try catchブロックを大量に入れるというのは
死んだ人間に釘を打ち付け何かに固定し立たせるのと似ている。
その異常なメカニズムは破棄して、
代わりに最小限の例外処理と通知をするだけの堅牢なメカニズムを組み込みます。

# 28. [「魔法」に頼りすぎてはいけない](https://プログラマが知るべき97のこと.com/エッセイ/魔法-に頼りすぎてはいけない)

[ (英文=> by AlanGriffiths)](http://programmer.97things.oreilly.com/wiki/index.php/Don%27t_Rely_on_%22Magic_Happens_Here%22)
自分の知らない仕事、自分の直接関わっていない仕事をしている人を尊重するということが大事です
自分が積極的にかかわらない仕事に関しては、無意識のうちに簡単だと思ってしまうし、
まるで「魔法」のように自動的に出来るような錯覚に陥ってしまうのが人間の常です。
順調なときは、魔法だと思っていても差し支えありません。
問題は魔法が解けた時です。魔法が解けてしまえば、とたんにプロジェクトは
頓挫し、混乱してしまいます。
魔法とな有能な人が混乱なく回していて、問題が起きていない状態など。
その有能な人を外しても大丈夫ではと思って外してみたら混乱に陥った。

# 29. [DRY原則](https://プログラマが知るべき97のこと.com/エッセイ/DRY原則)

[ (英文=> by Steve Smith)](http://programmer.97things.oreilly.com/wiki/index.php/Don%27t_Repeat_Yourself)
Don't Repeat Yourself 繰り返しを避けること。
重複箇所を一箇所にまとめれば、修正など一箇所ですみます。
作業の重複は自動化で防ぐ
ロジックの重複は抽象化で防ぐ
デザインパターンの活用や、データベースを正規化する。

# 30. [そのコードに触れてはならない！](https://プログラマが知るべき97のこと.com/エッセイ/そのコードに触れてはならない)

[ (英文=> by Cal Evans)](http://programmer.97things.oreilly.com/wiki/index.php/Don%27t_Touch_that_Code%21)
ローカル開発環境
総合テスト環境
品質保証、顧客が受け入れテストを行うステージングサーバー
本番環境
プログラマは、これらの環境のうち開発サーバーよりあとの環境に触れるべきではない。
問題が起きた場合でも、それを修正するのは基本的に運用チームの仕事であり、
仮に開発者が修正に当たるにしても、それは運用チームからの依頼であるべきです。

# 31. [状態だけでなく「ふるまい」もカプセル化する](https://プログラマが知るべき97のこと.com/エッセイ/状態だけでなく-ふるまい-もカプセル化する)

[ (英文=> by Einar Landre)](http://programmer.97things.oreilly.com/wiki/index.php/Encapsulate_Behavior%2C_not_Just_State)
オブジェクトは状態とふるまいの両方をカプセル化出来ます。
オブジェクトが元来どういう特性を持っているか すべきことはこの2つしか無い
オブジェクトへの責務の割当
他のオブジェクトへの責務の委譲

- [ドメインモデル貧血症](
http://bliki-ja.github.io/AnemicDomainModel/)
- [AnemicDomainModel](https://martinfowler.com/bliki/AnemicDomainModel.html)


# 32. [浮動小数点数は実数ではない](https://プログラマが知るべき97のこと.com/エッセイ/浮動小数点数は実数ではない)

[ (英文=> by Chuck Allison)](http://programmer.97things.oreilly.com/wiki/index.php/Floating-point_Numbers_Aren%27t_Real)
実数は精度は無限
浮動小数点数の精度は有限 実数というよりむしろ整数に近い
誤差が生じることは避けられない
どういう時に丸めの誤差が出るかをよく知り、その知識を踏まえた上でコーディングする。

# 33. [オープンソースプロジェクトで夢を実現する](https://プログラマが知るべき97のこと.com/エッセイ/オープンソースプロジェクトで夢を実現する)

[ (英文=> by Richard Monson-Haefel)](http://programmer.97things.oreilly.com/wiki/index.php/Fulfill_Your_Ambitions_with_Open_Source)
本当に自分の希望通りのソフトウェアを作ることの出来る立場にいる人は多くない。
希望に近づく方法はオープンソースプロジェクトに参加する。
他人の作ったソフトェアを学ぶのにテストコードを書くほど効果的な方法はないのです。

# 34. [API設計の黄金律](https://プログラマが知るべき97のこと.com/エッセイ/API設計の黄金律)

[ (英文=> by Michael Feathers)](http://programmer.97things.oreilly.com/wiki/index.php/The_Golden_Rule_of_API_Design)
黄金律「APIを提供するときは、API自身のテストだけでなく、必ずAPIを利用するコードの
ユニットテストも書く」
APIを開発する側が「APIを利用するコードのユニットテストは難しい」と認識すること。

- [パターン指向リファクタリング入門-ソフトウエア設計を改善する27の作法-ジョシュア・ケリーエブスキー](http://amzn.to/2A1sHnC)
- [Refactoring to Patterns (Addison-Wesley Signature Series (Fowler))](http://amzn.to/2yWcDWr)
- [EFFECTIVE-JAVA-Java-Joshua-Bloch](http://amzn.to/2yXkwL8)
- [Effective Java (Second Edition)](http://amzn.to/2zZG9Z3)
- [Effective Java (3rd Edition): Joshua Bloch](http://amzn.to/2yVWIav)

# 35. [超人の神話](https://プログラマが知るべき97のこと.com/エッセイ/超人の神話)

[ (英文=> by Ryan Brush)](http://programmer.97things.oreilly.com/wiki/index.php/The_Guru_Myth)
何も情報を与えられなくても、あらゆる質問に答え、あらゆる問題を解決できる、そんな人はいません。
彼らは頭は良いですが普通の人間です。
手間をかけてでも現状についての情報を十分に集め、その人に伝えます。
情報が十分に与えられれば、彼らは持てる力を存分に発揮できます。
スタックトレース、エラーログ、問題の起きた状況について詳しく説明するなど。
超人は必要ありません、必要なのはエキスパートです、
積極的に自分以外にもエキスパートを育てようとする意思を持ったエキスパートです。

# 36. [ハードワークは報われない](https://プログラマが知るべき97のこと.com/エッセイ/ハードワークは報われない)

[ (英文=> by Olve Maudal)](http://programmer.97things.oreilly.com/wiki/index.php/Hard_Work_Does_not_Pay_Off)
仕事には長い時間をかけず、集中して短い時間で終わらせるよう心がける
より効率的な問題解決方法を探す努力を常にする。
プロの仕事には、入念な準備と効率化のための努力、そして日々の反省と
絶え間ない変化が必要なのです。

# 37. [バグレポートの使い方](https://プログラマが知るべき97のこと.com/エッセイ/バグレポートの使い方)

[ (英文=> by Matt Doar)](http://programmer.97things.oreilly.com/wiki/index.php/How_to_Use_a_Bug_Tracker)
バグレポートには必ず次の3つを書く必要があります。
できるだけ詳しいバグの再現方法と発生頻度
本来の仕様（バグがない場合の望ましい動作。こうあるべき、と言う自分の意見で構わない）
実際の動作（完全でなくても、自分の記録した範囲で詳しく書く）
「バグ数は何かの単位、基準ではない」
コードの行数が労力を示していないと同じです。

# 38. [余分なコードは決して書かない](https://プログラマが知るべき97のこと.com/エッセイ/余分なコードは決して書かない)

[ (英文=> by Pete Goodliffe)](http://programmer.97things.oreilly.com/wiki/index.php/Improve_Code_by_Removing_It)
「より少ないことは、より豊かなこと（Less is more）」
YAGNI（You Ain't Gonna Need It それは多分、必要ない）
そもそもなぜ余計なコードが書かれたのか？レビューやペア作業でも見過ごされたのか？
おそらく次のような理由だろう。
余計かもしれないが、面白そうだと思えた
将来必要になるかもしれないと思った。そのためにはいま書くのがベストだと思った
必要かどうか判断に迷った。
顧客に判断を仰ぐべきだったが、それよりも実装してしまう方が簡単だと思った。
余分な機能を正当化するため、議論を経ておらず、ドキュメントにも書かれていない要件を
プログラマがでっち上げた。
・・・常に考える必要があるのです、今自分が書いているコードは本当に
必要なものなのか、と。

- [YagNi](http://wiki.c2.com/?YagNi)

# 39. [最初が肝心](https://プログラマが知るべき97のこと.com/エッセイ/最初が肝心)

[ (英文=> by Marcus Baker)](http://programmer.97things.oreilly.com/wiki/index.php/Install_Me)
人が何かをする時には、費用対効果が非常に大切な要素になります。
皆自分の中に基準があって、費用対効果がその基準を上回りそうな行動は取りますが
それを使うのに手間がかかりすぎると判断すれば、他のもっと手間のかからないものを探すでしょう。
つまり、有用性が同じであれば、手間のかからないものほど有利ということです。

# 40. [プロセス間通信とアプリケーションの応答時間の関係](https://プログラマが知るべき97のこと.com/エッセイ/プロセス間通信とアプリケーションの応答時間の関係)

[ (英文=> by Randy Stafford)](http://programmer.97things.oreilly.com/wiki/index.php/Inter-Process_Communication_Affects_Application_Response_Time)
応答時間をできるだけ短くしたほうがユーザー体験は良い。
その工夫を優先して行うほうが良い。

- [エンタープライズ-アプリケーションアーキテクチャパターン-Object-Oriented-SELECTION](http://amzn.to/2A0JGGn)
- [Patterns of Enterprise Application Architecture (Addison-Wesley Signature Series (Fowler)): Martin Fowler](http://amzn.to/2zXWBsR)
- [P of EAA: Lazy Load](https://martinfowler.com/eaaCatalog/lazyLoad.html)
- [オッカムの剃刀 - Wikipedia](https://ja.wikipedia.org/wiki/オッカムの剃刀)

# 41. [無駄な警告を排除する](https://プログラマが知るべき97のこと.com/エッセイ/無駄な警告を排除する)

[ (英文=> by Johannes Brodwall)](http://programmer.97things.oreilly.com/wiki/index.php/Keep_the_Build_Clean)
警告が出たらどんな小さいものでも潰していく。

# 42. [コマンドラインツールを使う](https://プログラマが知るべき97のこと.com/エッセイ/コマンドラインツールを使う)

[ (英文=> by Carroll Robinson)](http://programmer.97things.oreilly.com/wiki/index.php/Know_How_to_Use_Command-line_Tools)
IDEを使っていると裏で何をやっているかわからない。
コマンドラインツールならば何をしているのか分かる。
コマンドラインツールは時にはIDEよりも便利な場合がある。
簡単に自動化出来る。
IDEを使うなとは言っていません、IDEが裏でしていることをよく見て理解しよう。
ということです。

# 43. [プログラミング言語は複数習得すべき](https://プログラマが知るべき97のこと.com/エッセイ/プログラミング言語は複数習得すべき)

[ (英文=> by Russel Winder)](http://programmer.97things.oreilly.com/wiki/index.php/Know_Well_More_than_Two_Programming_Languages)
第二の言語には最初の言語とはパラダイムの違う言語を選ぶべきです。
パラダイムの違う言語を学ぶと、アルゴリズム、イディオム、パターンの実装について
嫌でも考えるようになるからです。
この体験がプログラマの技術を大きく向上させます。
第二言語を1週間学ぶのでは不十分です、数ヶ月もの間、毎日少しでも
その言語に触れる必要があるでしょう。
大事なのはその言語のイディオムを身につけることです。

- [データフロープログラミング - Wikipedia](https://ja.wikipedia.org/wiki/データフロープログラミング)

# 44. [IDEを知る](https://プログラマが知るべき97のこと.com/エッセイ/IDEを知る)

[ (英文=> by Heinz Kabutz)](http://programmer.97things.oreilly.com/wiki/index.php/Know_Your_IDE)
昔はテキストエディタだけでした、
気に入っているのは自動リファクタリング機能、メソッド抽出
これは、メソッドの中の中の一部のコードを選ぶと、その部分を新たなメソッドとして
切り出してくれる機能です。
他に、新たに作ったメソッドで置換可能な箇所が既存のコードの中にないか探す機能もあります。
コーディング規約を強制的に守らせる機能もあります。
IDEを使い始める時最初にショートカットを覚えます。覚えておくと思考の流れを
中断せずに作業が進められます。
IDEを時間をかけて学んでいくべきでしょう。

# 45. [限界を知る](https://プログラマが知るべき97のこと.com/エッセイ/限界を知る)

[ (英文=> by Greg Colvin)](http://programmer.97things.oreilly.com/wiki/index.php/Know_Your_Limits)
限界が具体的にどのくらいかを知る。
自分自身の限界
プロジェクトチームのメンバーたちの限界
予算の限界
自分の持つ時間
ハードウェア、ツールの限界
ソフトウェア技術者の場合
自分の使うシステムの、データ構造、アルゴリズム、アーキテクチャ、性能などの特性の
空間と時間の複雑性を知ることが重要になります。
ソフトウェアとハードウェアの最適な組み合わせを見つけて、両者の力を
最大限に引き出すのです。

- [Mans Got To Know His Limitations - YouTube](https://www.youtube.com/watch?v=t2JnCXvm_Qc)
- [Van Emde boas tree - Wikipedia](https://en.wikipedia.org/wiki/Van_Emde_boas_tree)
- [ON LANGUAGE - You Pays Yer Money - NYTimes.com](http://www.nytimes.com/1988/02/28/magazine/on-language-you-pays-yer-money.html?pagewanted=all)

# 46. [すべきことは常に明確に](https://プログラマが知るべき97のこと.com/エッセイ/すべきことは常に明確に)

[ (英文=> by Dan Bergh Johnsson)](http://programmer.97things.oreilly.com/wiki/index.php/Know_Your_Next_Commit)
全体を見渡し大目標、小目標とわけ 目的を明確にして作業時間を予測して
作業を行う。作業時間が予定以上に掛かりそうだとわかったら一旦中止をして
加えた変更をすべて破棄します。
そのあと、小目標を更に細かく分けて、再び新たな小目標を達成のための
作業を開始します。
コードは白紙に戻りますが、直前の作業から得た教訓、ひらめきは頭に残っているはずです
明確な目標もわからないのに闇雲に先を急ぐよりも、少し遠回りのようでも
確実に有効とわかる作業を探したほうが、結局は最終目標に向かって
着実に前に進むことになるからです。
大事なのは、常に自分が何をすべきかを明確にするということです。
完了する期限も必ず決めます

# 47. [大量のデータはデータベースで](https://プログラマが知るべき97のこと.com/エッセイ/大量のデータはデータベースで)

[ (英文=> by Diomidis Spinellis)](http://programmer.97things.oreilly.com/wiki/index.php/Large_Interconnected_Data_Belongs_to_a_Database)
アプリケーションで大量の永続データを扱う必要がある場合やデータが相互に
関係し合う場合は迷うことなくデータベースを使いましょう。

- [Dangling pointer - Wikipedia](https://en.wikipedia.org/wiki/Dangling_pointer)
- [Processing.org](https://processing.org/)

# 48. [いろいろな言葉を学ぶ](https://プログラマが知るべき97のこと.com/エッセイ/いろいろな言葉を学ぶ)

[ (英文=> by Klaus Marquardt)](http://programmer.97things.oreilly.com/wiki/index.php/Learn_Foreign_Languages)
他者とのコミュニケーションは大切。
カール大帝「他者の言葉を知ることは、新たな魂を持つこと」
他の業界の人とコミュニケーションをしてみれば、他の世界の言葉をしることの
大切さがよく分かるでしょう。
大事なのは自分が話すこと以上に、相手の話に耳を傾けることです。
言葉にならない言葉の存在を知ることが大事なのです。

# 49. [見積りとは何か](https://プログラマが知るべき97のこと.com/エッセイ/見積りとは何か)

[ (英文=> by Giovanni Asproni)](http://programmer.97things.oreilly.com/wiki/index.php/Learn_to_Estimate)
見積り 見積りのために事実の裏付けに基づく推量が必要
ターゲット 実現したいビジネス上の目標を明文化したもの
コミットメント ある機能を、ある期日までに一定上の品質で提供すると約束すること
ソフトウェアの見積りの主目的は、プロジェクトの結果を予言することではない。
見積もりを行うのは、プロジェクトのターゲットがコントロールによって達成可能な
程度に現実的なものかどうかを判断するためである。

- [ソフトウェア見積り | スティーブ マコネル, 久手堅 憲之, Steve McConnell, 田沢 恵, 溝口 真理子](http://amzn.to/2yX4S2r)
- [Software Estimation: Demystifying the Black Art (Developer Best Practices): Steve McConnell](http://amzn.to/2yX5W6j)

# 50. [Hello, Worldから始めよう](https://プログラマが知るべき97のこと.com/エッセイ/Hello,-Worldから始めよう)

[ (英文=> by Thomas Guest)](http://programmer.97things.oreilly.com/wiki/index.php/Learn_to_Say_%22Hello%2C_World%22)
彼は問題の巨大な関数の中の一部を切り出して関数にラッピングしました。
そして、彼は永久にループするmain関数を書きました。
永久にループし、ユーザーに値の入力を求めるコードです。
$ cc tryit.c && ./a.out
今ならテスト駆動開発を勧める。

- [プログラミング言語C 第2版 ANSI規格準拠 | B.W. カーニハン, D.M. リッチー, 石田 晴久](http://amzn.to/2hmJARW)
- [C Programming Language (Prentice Hall Software): Brian W. Ritchie, Dennis Kernighan](http://amzn.to/2zQMaGv)

# 51. [プロジェクト自身にしゃべらせる](https://プログラマが知るべき97のこと.com/エッセイ/プロジェクト自身にしゃべらせる)

[ (英文=> by Daniel Lindner)](http://programmer.97things.oreilly.com/wiki/index.php/Let_Your_Project_Speak_for_Itself)
自動化の勧め
CI
XFD(eXtreme Feedback Device)

# 52. [「その場しのぎ」が長生きしてしまう](https://プログラマが知るべき97のこと.com/エッセイ/その場しのぎ-が長生きしてしまう)

[ (英文=> by Klaus Marquardt)](http://programmer.97things.oreilly.com/wiki/index.php/The_Longevity_of_Interim_Solutions)
暫定ソリューション＝その場しのぎ
一旦出来てしまうと既成事実化してしまう。
対応は大きく分けて3つ
暫定ソリューションをはじめから一切作らない
暫定ソリューション修正の優先度が上がる体制づくりをする。
プロジェクトマネージャーが自然に暫定ソリューションの修正を
より優先するような体制にする。
現状のまま何も変えない
暫定ソリューションが使い続けられている状況を変える最善の方法は
暫定ソリューションを不要にしてしまうことです。
後から改めてより優れたソリューション、より有用性の高いソリューションを
作るのです。
大事なのは、自分に変えられることと、変えられないことを冷静に見極めることです。
そして、変えられることは勇気を持って変える。その姿勢で挑めば成果は上がるでしょう。

# 53. [正しい使い方を簡単に、誤った使い方を困難に](https://プログラマが知るべき97のこと.com/エッセイ/正しい使い方を簡単に-誤った使い方を困難に)

[ (英文=> by Scott Meyers)](http://programmer.97things.oreilly.com/wiki/index.php/Make_Interfaces_Easy_to_Use_Correctly_and_Hard_to_Use_Incorrectly)
インタフェース使用を決定する作業は必ず必要です。
良いインタフェースとは次の2条件を満たすことです。
正しく使用するほうが操作ミスをするより簡単。
誤った使い方をすることが困難。
良いインタフェースを設計するにはコードを書く前にシミュレーションしてみます。
使い方を間違えにくインタフェースをつくるには、
ユーザーがしそうな間違いを事前に予測し、それを防止する策を講じることです。
リリースの早い時期に実際にインタフェースがどのように誤用されるかを観察し、
改良を加えることです。
何より重要なのは、インタフェースが存在するのはユーザーの利便のためであり、
開発側の利便のためではないということです、それを忘れてはなりません。

# 54. [見えないものを見えるように](https://プログラマが知るべき97のこと.com/エッセイ/見えないものを見えるように)

[ (英文=> by Jon Jagger)](http://programmer.97things.oreilly.com/wiki/index.php/Make_the_Invisible_More_Visible)
ソースコードは実態を持っていません。
プログラムを実行してもソースコードが目に見えるわけではありません。
バグを修正している間は開発は前に進みません。
デバック作業を具体的にどういうことをしていて、どのくらい時間がかかるか
目に見えるようにするべきです。
進捗も見えるようにするべきです。
人間は目に見えるもの、具体的な形のあるものについてはよく考えますが、
そうでないものについてはあまり考えない傾向にあるのです。
対処法
ユニットテストを書く
ユニットテストを実行する。
プロジェクトの進捗を掲示板やカードで視覚化します。
インクリメンタル開発の手法を使う
ソフトウェア開発プロジェクトを進める際はいつでも、目に見える証拠が
たくさんあるという状態を維持すべきでしょう。

- [ほとんど無害-河出文庫-ダグラス・アダムス](http://amzn.to/2hnhtBT)

# 55. [並行処理に有効なメッセージパッシング](https://プログラマが知るべき97のこと.com/エッセイ/並行処理に有効なメッセージパッシング)

[ (英文=> by Russel Winder)](http://programmer.97things.oreilly.com/wiki/index.php/Message_Passing_Leads_to_Better_Scalability_in_Parallel_Systems)
並行処理を書くのは難しい。
その根幹は共有メモリである。
共有メモリを使わずメッセージパッシングを使ってプログラミングをすることが、
現在のコンピュータハードウェアにはどうしても必要な並行／並列処理にとって
最も有効な方法だといえるでしょう。

- [Occam - Wikipedia](https://ja.wikipedia.org/wiki/Occam)
- [Communicating Sequential Processes - Wikipedia](https://ja.wikipedia.org/wiki/Communicating_Sequential_Processes)
- [データフロー - Wikipedia](https://ja.wikipedia.org/wiki/データフロー)

# 56. [未来へのメッセージ](https://プログラマが知るべき97のこと.com/エッセイ/未来へのメッセージ)

[ (英文=> by Linda Rising)](http://programmer.97things.oreilly.com/wiki/index.php/A_Message_to_the_Future)
難しいものは難しいコードになると思っているのでは？
書いた本人さえ理解が難しくなる。そんなコードを書いても変だと思わないようです。
自分の書くコードは全部、未来の誰かへのメッセージだと思うのよ。
その誰かは、あなたの弟さんかもしれないし。誰か、とても賢い人に、
自分の難しい問題をどうやって解いたのか、丁重に説明するつもりで書くの。
想像してみて。いつか、誰か賢い人が、あなたの書いたコードを見て言うのよ。
「おおっ、これはすごい！何が書いてあるか完璧に分かる。
なんて簡潔でわかりやすいんだ。美しい。
本当に美しいコードだよ。傑作だ！皆に見せなくっちゃ」ってね。

# 57. [ポリモーフィズムの利用機会を見逃さない](https://プログラマが知るべき97のこと.com/エッセイ/ポリモーフィズムの利用機会を見逃さない)

[ (英文=> by Kirk Pepperdine)](http://programmer.97things.oreilly.com/wiki/index.php/Missing_Opportunities_for_Polymorphism)
ポリモーフィズムとは、同じクラスのオブジェクトやメソッドが複数の形を
とり得るということを意味します。
しかし、ポリモーフィズムは、ただ単に実装が複数になるということを
意味しているのではありません。
うまく使えば、オブジェクトやメソッドの特性、動きをコンテキストに応じて
細かく変えることが出来ます。
しかも、そのために助長なif-then-elseブロックを書く必要が無いのです。
そのかわり、コンテキストによってオブジェクトやメソッドが自動的に形を変えるためには。
「このコンテキストならこのオブジェクト、あるいはメソッドを使う」
と言うコードをあらかじめコンテキストの外で書いておく必要があります。
ポリモーフィズムを有効に活かせば、その分コードの量が減り、読みやすくなります。
今、コードの中にif-then-elseブロックがあるのなら、
そのすべてについてポリモーフィズムが使えないか検討したほうが良い、
と言ってもいいでしょう。

# 58. [テスト担当者はプログラマの友人](https://プログラマが知るべき97のこと.com/エッセイ/テスト担当者はプログラマの友人)

[ (英文=> by Burk Hufnagel)](http://programmer.97things.oreilly.com/wiki/index.php/News_of_the_Weird:_Testers_Are_Your_Friends)
コードを書く人と、テストをする人が分かれていた場合、
敵ではなく友人です。

# 59. [バイナリは常に1つ](https://プログラマが知るべき97のこと.com/エッセイ/バイナリは常に1つ)

[ (英文=> by Steve Freeman)](http://programmer.97things.oreilly.com/wiki/index.php/One_Binary)
皆がどの環境でも常に同じバイナリを利用するようにする。
環境に関する情報もバージョン管理をする。
現在ならDockerやVagrant等。

# 60. [真実を語るはコードのみ](https://プログラマが知るべき97のこと.com/エッセイ/真実を語るはコードのみ)

[ (英文=> by Peter Sommerlad)](http://programmer.97things.oreilly.com/wiki/index.php/Only_the_Code_Tells_the_Truth)
要件定義書や設計書が正確に書かれていてもそれが真実をすべて語ってくれるわけではありません。
手がかりはソースコードだけ。
読んでわかりやすいソースコードを書きましょう。
重要なのは名前の付け方
テストを書く。
リファクタリングをする。
コードを書くとは、相手にわかりやすく。手紙を書いたりブログを書くのと同じように。
書いた本人がそばにいて逐一説明する必要が無いように書く。

# 61. [ビルドをおろそかにしない](https://プログラマが知るべき97のこと.com/エッセイ/ビルドをおろそかにしない)

[ (英文=> by Steve Berczuk)](http://programmer.97things.oreilly.com/wiki/index.php/Own_%28and_Refactor%29_the_Build)
きれいなコードを書く人でもビルドスクリプトは疎かにしがちです。
質の高いビルドスクリプトを書きましょう。
そうすれば、ビルドの手間を省き、皆がコーディングに集中することができ、
作業がより楽しいものになります。

# 62. [プリミティブ型よりドメイン固有の型を](https://プログラマが知るべき97のこと.com/エッセイ/プリミティブ型よりドメイン固有の型を)

[ (英文=> by Einar Landre)](http://programmer.97things.oreilly.com/wiki/index.php/Prefer_Domain-Specific_Types_to_Primitive_Types)
ドメイン固有の型を積極的に使う。

# 63. [ユーザの操作ミスを防止する](https://プログラマが知るべき97のこと.com/エッセイ/ユーザの操作ミスを防止する)

[ (英文=> by Giles Colborne)](http://programmer.97things.oreilly.com/wiki/index.php/Prevent_Errors)
エラーメッセージはユーザーとシステム感の重要なコミュニケーション手段です。
ユーザーのミスを事前に予防することも可能。
ユーザーとシステム間のコミュニケーションの「デバッグ」と考えます。
システムはユーザーの操作ミスに関して寛容であるべきです。

# 64. [プロのプログラマとは？](https://プログラマが知るべき97のこと.com/エッセイ/プロのプログラマとは)

[ (英文=> by Uncle Bob)](http://programmer.97things.oreilly.com/wiki/index.php/The_Professional_Programmer)
プロフェッショナルなプログラマの最大の特徴は「自分が責任を取る」という態度、
責任感です。
まず、自らのキャリアに責任を持ちます。
責任の取れないような見積りやスケジューリングは決してせず、作る製品の質にも責任を持ちます。
ミスがあれば自ら対応します。他人に責任を押し付けるような
ことは一切しない、それがプロです。

# 65. [バージョン管理システムを有効に使う](https://プログラマが知るべき97のこと.com/エッセイ/バージョン管理システムを有効に使う)

[ (英文=> by Diomidis Spinellis)](http://programmer.97things.oreilly.com/wiki/index.php/Put_Everything_Under_Version_Control)
仕事に関係のあるファイルを、とにかくなんでもバージョン管理の対象にすべきでしょう。
意味のある変更を加えるたびにコミットする。
まとめてコミットはしない。
コミットする際必ず説明を添える。
少なくともどのような変更したのか簡単な説明を加えること。
なぜ変更したのかという理由も書いておくと良い。
ビルドを壊すようなコミットをしないこと。

# 66. [いったんコンピュータから離れてみる](https://プログラマが知るべき97のこと.com/エッセイ/いったんコンピュータから離れてみる)

[ (英文=> by Burk Hufnagel)](http://programmer.97things.oreilly.com/wiki/index.php/Put_the_Mouse_Down_and_Step_Away_from_the_Keyboard)
何時間も集中して考えているのに、問題が難しくなかなか解決策が思いつかない。
そんな時、散歩に出かけたり、自動販売機まで何かを買いに行ったりしたら、
帰りに突然答えがわかったという経験をした人は案外多いのではないでしょうか？
これは、コーディング中は脳の論理を司る部分だけが働いていて、
想像を司る部分が働いていないためではないかと私は考えています。

# 67. [コードを読む](https://プログラマが知るべき97のこと.com/エッセイ/コードを読む)

[ (英文=> by Karianne Berg)](http://programmer.97things.oreilly.com/wiki/index.php/Read_Code)
コードを書くのは楽しいのに、読むのは辛い。
他人が書いたコードがひどいからではなく、思考や問題解決の方法が自分とは違っているからです。
しかし、意外かもしれませんが、実は他人の書いたコードを読むことは
自分の成長につながるのです。
プログラミングの技術を本気で磨きたいと思っているのなら、
本を読むのもいいですが、一番いいのは、他人が書いたものでも
自分か書いたものでも、とにかくコードを読むことです。

- [レガシーコード改善ガイド (Object Oriented SELECTION) | マイケル・C・フェザーズ, ウルシステムズ株式会社, 平澤 章, 越智 典子, 稲葉 信之, 田村 友彦, 小堀 真義](http://amzn.to/2hnk66J)
- [Working Effectively With Legacy Code: Michael Feathers](http://amzn.to/2zQR8TG)
- [Code Reading ~オープンソースから学ぶソフトウェア開発技法~ (プレミアムブックス版) | Diomidis Spinellis, まつもと ゆきひろ, 平林 俊一, 鵜飼 文, トップスタジオ](http://amzn.to/2yWveSl)

# 68. [「人間」を知る](https://プログラマが知るべき97のこと.com/エッセイ/人間-を知る)

[ (英文=> by Keith Braithwaite)](http://programmer.97things.oreilly.com/wiki/index.php/Read_the_Humanities)
よほど小規模なプロジェクトは別にして、必ず人と人が仕事をすることになります。
しかし、プログラマーが人との関わりについて教育を受けることは、
残念なことに殆どありません。

# 69. [車輪の再発明の効用](https://プログラマが知るべき97のこと.com/エッセイ/車輪の再発明の効用)

[ (英文=> by Jason P Sage)](http://programmer.97things.oreilly.com/wiki/index.php/Reinvent_the_Wheel_Often)
再利用をする方が安全でコストが少なくすみます。
しかしそれでは自分は中身を知ることもなく、自分自身も成長しません。
車輪の再発明をしようとした結果、失敗することもあるでしょう、
しかし、それは貴重な体験となるでしょう。
自分の手でゼロからコードを書き、あれこれ試行錯誤することを通して学ぶのは、
ただ単に技術書を読んで学ぶこととは大きく違います。
本を通して知識を得ることは大切です、しかし、優れたプログラマーになるためには、
経験を積むことがどうしても必要です。

# 70. [シングルトンパターンの誘惑に負けない](https://プログラマが知るべき97のこと.com/エッセイ/シングルトンパターンの誘惑に負けない)

[ (英文=> by Sam Saariste)](http://programmer.97things.oreilly.com/wiki/index.php/Resist_the_Temptation_of_the_Singleton_Pattern)
シングルトンパターンは利点よりも弊害が多い。
利点、クラスのインスタンスは一つしか生成されない、使用前にかならず初期化される、
グローバルアクセスポイントとすることで設計をシンプルに出来る。
問題点、テストの妨げ、保守性の点でも不利、
必要なインスタンスは一つだけと言う要望は、多くの場合推測にすぎない。
理論的には独立しているはずのコード間に暗黙の依存関係を生んでしまう。
シングルトンパターンは永続化された状態を暗黙のうちに伴う。
マルチスレッド環境での使用は特に危険が大きい。
シングルトンはクリーンアップに関しても問題を起こしやすい。
シングルトンを明示的に殺すための機能はありません。
プログラム終了の際には、シングルトンも自動的にクリーンアップされることになります。

# 71. [パフォーマンスへの道は地雷コードで敷き詰められている](https://プログラマが知るべき97のこと.com/エッセイ/パフォーマンスへの道は地雷コードで敷き詰められている)

[ (英文=> by Kirk Pepperdine)](http://programmer.97things.oreilly.com/wiki/index.php/The_Road_to_Performance_Is_Littered_with_Dirty_Code_Bombs)
ホットスポット＝プログラムの実行時間の80%はコードの20%で実行される、と言われる。
ホットスポットを見つけ、パフォーマンスを向上させようとする。
見積りで3-4時間でと思っていたが依存関係があり3-4週間になってしまうなどと
そういうことはよくあるのです。
実は、コードの依存性、複雑さを計測する手段や、それをコントロールするための手段というのは数多くあります。
ソフトウェアメトリクスを使用すると、コードの様々な特性を定量的に
評価した指標のことです。
このようなツールを使い、パフォーマンスチューニングの作業に深刻な悪影響を
及ぼす前にコードの地雷を発見し排除するのです。

# 72. [シンプルさは捨てることによって得られる](https://プログラマが知るべき97のこと.com/エッセイ/シンプルさは捨てることによって得られる)

[ (英文=> by Paul W. Homer)](http://programmer.97things.oreilly.com/wiki/index.php/Simplicity_Comes_from_Reduction)
ある程度以下の質のコードは即座に破棄した方がいい。
良い部分を残し、悪い部分を消すという作業が難しいのなら、全部破棄して
初めから書き直すほうがいいのです。
せっかく書いたものを結局全部消したという記憶が頭の何処かにあれば、
次からは無駄なコードを書かないでおこうと無意識に気をつけるようになるはずです。

# 73. [単一責任原則](https://プログラマが知るべき97のこと.com/エッセイ/単一責任原則)

[ (英文=> by Uncle Bob)](http://programmer.97things.oreilly.com/wiki/index.php/The_Single_Responsibility_Principle)
良いデザインの基本原則
変更する理由が同じものは集める、変更する理由が違うものは分ける。
単一責任原則(Single Responsibility Principle SRP)と呼ばれています。
一つの関数に変更する理由は一つのみにする。

- [アジャイルソフトウェア開発の奥義 第2版 オブジェクト指向開発の神髄と匠の技 | ロバート・C・マーチン, Robert C. Martin, 瀬谷 啓介](http://amzn.to/2yYcvWs)
- [Agile Software Development, Principles, Patterns, and Practices: Pearson New International Edition: Robert C. Martin](http://amzn.to/2ho0uPX)

# 74. [「イエス」から始める](https://プログラマが知るべき97のこと.com/エッセイ/-イエス-から始める)

[ (英文=> by Alex Miller)](http://programmer.97things.oreilly.com/wiki/index.php/Start_from_Yes)
「イエス」と言う返答から始めるようにすれば、それだけ物の見方は大きく変わり
仕事の進め方も変わるだろう。
「イエス」から始めれば、人との対立は生まれず、協力関係が生まれるのです。

# 75. [面倒でも自動化できることは自動化する](https://プログラマが知るべき97のこと.com/エッセイ/面倒でも自動化できることは自動化する)

[ (英文=> by Cay Horstmann)](http://programmer.97things.oreilly.com/wiki/index.php/Step_Back_and_Automate%2C_Automate%2C_Automate)
よくある誤解
* 自動化はテストだけのもの
* IDEを使っていれば自動化の必要はない
* 自動化のためには特殊なツールについて学ぶ必要がある。
* 扱うファイル形式によっては自動化が出来ないことがある。
* 忙しくて自動化のことまで勉強している時間はない。

- [iMacros - Wikipedia](https://en.wikipedia.org/wiki/IMacros)
- [Selenium - Web Browser Automation](http://www.seleniumhq.org/)

# 76. [コード分析ツールを利用する](https://プログラマが知るべき97のこと.com/エッセイ/コード分析ツールを利用する)

[ (英文=> by Sarah Mount)](http://programmer.97things.oreilly.com/wiki/index.php/Take_Advantage_of_Code_Analysis_Tools)
テストは重要です、ですがテストだけがコードの品質を高める唯一の方法というわけではありません。
解析ツールは現在ではより便利になっていて積極的に使うべきでしょう。
Splint Pylint
独自のチェッカーを作ることにも恐れることなく挑戦してみてください。

- [Lint (software) - Wikipedia](https://en.wikipedia.org/wiki/Lint_(software))
- http://www.splint.org Not 404 Found
- [pylint (analyzes Python source code looking for bugs and signs of poor quality) (Logilab.org)](https://www.logilab.org/857)
- [ソフトウェア設計とは何か-原文-](http://knagano.tumblr.com/post/11941519742/ソフトウェア設計とは何か-原文-what-is-software)
- [ソフトウェア設計とは何か？ （原文： What Is Software... - knagano.tumblr.com](http://knagano.tumblr.com/post/11941519742/%E3%82%BD%E3%83%95%E3%83%88%E3%82%A6%E3%82%A7%E3%82%A2%E8%A8%AD%E8%A8%88%E3%81%A8%E3%81%AF%E4%BD%95%E3%81%8B-%E5%8E%9F%E6%96%87-what-is-software)
- [What Is Software Design? by Jack W. Reeves - developer.*, Developer Dot Star](https://www.developerdotstar.com/mag/articles/reeves_design.html)
- [世の世迷言: ソフトウェア工学とは何か](http://m-ksk.blogspot.jp/2006/10/blog-post.html)

# 77. [偶然の仕様ではなく本物の仕様のためのテストを書く](https://プログラマが知るべき97のこと.com/エッセイ/偶然の仕様ではなく本物の仕様のためのテストを書く)

[ (英文=> by Kevlin Henney)](http://programmer.97things.oreilly.com/wiki/index.php/Test_for_Required_Behavior%2C_not_Incidental_Behavior)
テストは厳格に書くべきですが、同時に本当にテストすべきことは何かをよく考え、
的確なものにする必要があるのです。
「テストを実施した」と言うだけで不当な安心感を持ってしまうことがあります。
ブラックボックステストを実施しましょう。

# 78. [テストは夜間と週末に](https://プログラマが知るべき97のこと.com/エッセイ/テストは夜間と週末に)

[ (英文=> by Rajith Attapattu)](http://programmer.97things.oreilly.com/wiki/index.php/Test_While_You_Sleep_%28and_over_Weekends%29)
巨大なプログラムにはテストに時間がかかります、それならば夜間や終末に
自動実行するようにしましょう。

# 79. [テストのないソフトウェア開発はあり得ない](https://プログラマが知るべき97のこと.com/エッセイ/テストのないソフトウェア開発はあり得ない)

[ (英文=> by Neal Ford)](http://programmer.97things.oreilly.com/wiki/index.php/Testing_Is_the_Engineering_Rigor_of_Software_Development)
ソフトウェアを開発する者にとって、テストをするということは、作る物に責任を持つということなのです。
テストはソフトウェア開発の中でも特に難しく、そして重要な部分と言っていいでしょう。

# 80. [1人より2人](https://プログラマが知るべき97のこと.com/エッセイ/1人より2人)

[ (英文=> by Adrian Wible)](http://programmer.97things.oreilly.com/wiki/index.php/Two_Heads_Are_Often_Better_than_One)
ペアプログラミングをしましょう。
ペアプログラミングには生産性、作業速度を40%向上させる効果があるという結果が得られています。

# 81. [エラーがエラーを相殺してしまう](https://プログラマが知るべき97のこと.com/エッセイ/エラーがエラーを相殺してしまう)

[ (英文=> by Allan Kelly)](http://programmer.97things.oreilly.com/wiki/index.php/Two_Wrongs_Can_Make_a_Right_%28and_Are_Difficult_to_Fix%29)
アポロ11号の月着陸船のソフトウェア設計をしたAllan Klumppはあるインタビューで
バグがあったことを明かしています、しかし、そのバグは別のバグによって相殺されたため
月着陸は無事成功しました。
複数の原因がある問題にどう対処すべきか、
まず大切なのは、そういう問題が存在し得ると認識することでしょう。
そして、思い込みを捨ててあらゆる対処を思いつくよう、冷静さを保つことが重要です。

- [Apollo Mission Software](https://www.netjeff.com/humor/item.cgi?file=ApolloComputer)

# 82. [他者への思いやりを意識したコーディング](https://プログラマが知るべき97のこと.com/エッセイ/他者への思いやりを意識したコーディング)

[ (英文=> by Aslam Khan)](http://programmer.97things.oreilly.com/wiki/index.php/Ubuntu_Coding_for_Your_Friends)
プログラマは一人で作業することが多い。孤立して作業をしていると、
このコードはいずれ他人によって使用され実行されるのだということを、つい忘れがちになります。
Ubuntuは元々ズールー語で「他者への思いやり」というような意味です。
どのような形であれ、そのコードに触れた誰もが、触れる前より良い人間、
良いプログラマになれる、そういうコードを書くようにすべきでしょう。

- [The leading operating system for PCs, IoT devices, servers and the cloud | Ubuntu](https://www.ubuntu.com/)
- [Homepage | Ubuntu Japanese Team](http://ubuntulinux.jp/)

# 83. [UNIXツールを友にする](https://プログラマが知るべき97のこと.com/エッセイ/UNIXツールを友にする)

[ (英文=> by Diomidis Spinellis)](http://programmer.97things.oreilly.com/wiki/index.php/The_Unix_Tools_Are_Your_Friends)
UNIXツールを使う。
いくつか簡単なルールを守ってプログラムを書きましょう。
* シングルタスクのプログラムであること。
* 標準入力からテキスト行としてデータを読み込むこと。
* 実行結果は標準出力に書き込み、その際ヘッダなどの余計な飾りは付けないこと。
* ツールの動作に影響するパラメーターはすべてコマンドラインに指定するようにしましょう。

- [Signature Survey](http://c2.com/doc/SignatureSurvey/)
- [BusyBox](https://busybox.net/)
- [Poems - If--](http://www.kiplingsociety.co.uk/poems_if.htm)

# 84. [正しいアルゴリズムとデータ構造を選ぶ](https://プログラマが知るべき97のこと.com/エッセイ/正しいアルゴリズムとデータ構造を選ぶ)

[ (英文=> by JC van Winkel)](http://programmer.97things.oreilly.com/wiki/index.php/Use_the_Right_Algorithm_and_Data_Structure)
［まずは動かすこと、速くするのはその後でいい」
適切なアルゴリズムを選ぶ
適切なデータ構造を選ぶ
そのためには問題領域と、アルゴリズム、データ構造の十分な知識が必要。

# 85. [冗長なログは眠りを妨げる](https://プログラマが知るべき97のこと.com/エッセイ/冗長なログは眠りを妨げる)

[ (英文=> by Johannes Brodwall)](http://programmer.97things.oreilly.com/wiki/index.php/Verbose_Logging_Will_Disturb_Your_Sleep)
ログは綺麗に、大量のログはログが無いのと同じ。
エラーログには重大な問題以外記録されないようにしておく。
通常時のエラーログには何も記録されないくらいのほうがいいといえます。

# 86. [WETなシステムはボトルネックが見つかりにくい](https://プログラマが知るべき97のこと.com/エッセイ/WETなシステムはボトルネックが見つかりにくい)

[ (英文=> by Kirk Pepperdine)](http://programmer.97things.oreilly.com/wiki/index.php/WET_Dilutes_Performance_Bottlenecks)
DRY原則 ＝Don't Repeat Yourself 同じことを繰り返すな。
DRY原則に反しているシステムをWETなシステム（＝Write Every Time 必要な物をその都度書く）
DRY原則を守ることで、パフォーマンスのボトルネックの発見と解消が、
WETなコードの場合より容易になっているということです。

# 87. [プログラマとテスターが協力してできること](https://プログラマが知るべき97のこと.com/エッセイ/プログラマとテスターが協力してできること)

[ (英文=> by Janet Gregory)](http://programmer.97things.oreilly.com/wiki/index.php/When_Programmers_and_Testers_Collaborate)
テスターとプログラマーが協力し合えば奇跡が生まれます。
テストをコーディング開始前に受け取ればテスト駆動開発が出来ます。
時間に余裕ができ、その分ソフトウェアの機能をより充実させることが出来ます。
さらにもう一歩進めて、プログラマーがコーディングを始める前に、
テスターは「どういうテストをするつもりか」という考えを伝えるだけでなく、同時に、
プログラマーに何か提案はないかと尋ねるのです。
そうすれば、テストカバレッジをあげるのに役立つ情報、あるいは、
どれが必要なテストでどれが不要なテストかの見極めに役立つ情報が
提供されることが多いのです。
バグの発生を未然に防ぐ事ができ、時間の節約もできるのです。
両者は自動化に関しても協力し合うことが出来ます。

- [Wiki: Welcome Visitors](http://fit.c2.com/)

# 88. [コードは生涯サポートするつもりで書く](https://プログラマが知るべき97のこと.com/エッセイ/コードは生涯サポートするつもりで書く)

[ (英文=> by Yuriy Zubarev)](http://programmer.97things.oreilly.com/wiki/index.php/Write_Code_as_If_You_Had_to_Support_It_for_the_Rest_of_Your_Life)
いつも「このコードは生涯、自分がサポートし続けなくてはならない」
と思ってコードを書く。
「ベストプラクティス」を学びずっと守り続けること。
このコードは自分の今後の人生を決めるのだ、と思って書くべきでしょう。

# 89. [関数の「サイズ」を小さくする](https://プログラマが知るべき97のこと.com/エッセイ/関数の-サイズ-を小さくする)

[ (英文=> by Keith Braithwaite)](http://programmer.97things.oreilly.com/wiki/index.php/Write_Small_Functions_Using_Examples)
正しいコードを書きたいというのは誰もが思うことです、そして自分の書いたコードが
間違いなく正しいと言う証拠も欲しいでしょう。
そういう意味で役立つのは、関数の「サイズ」という指標です。
コードの量という意味ではなく、そのコードが表現している数学関数のサイズという意味です。

- [xUnit Test Patterns: Refactoring Test Code (Addison-Wesley Signature Series (Fowler)): Gerard Meszaros](http://amzn.to/2gWfAiL)
- [新装版 リファクタリング―既存のコードを安全に改善する― (OBJECT TECHNOLOGY SERIES) | Martin Fowler, 児玉 公信, 友野 晶夫, 平澤 章, 梅澤 真史](http://amzn.to/2yVNriR)
- [Refactoring: Improving the Design of Existing Code (Addison-Wesley Object Technology Series): Martin Beck, Kent Brant, John Opdyke, William Roberts, Don Fowler](http://amzn.to/2yX1zbq)

# 90. [コードを見る人のためにテストを書く](https://プログラマが知るべき97のこと.com/エッセイ/コードを見る人のためにテストを書く)

[ (英文=> by Gerard Meszaros)](http://programmer.97things.oreilly.com/wiki/index.php/Write_Tests_for_People)
テストはいつもコードを書き始める前に書くようにしている、という人は素晴らしい。
しかし、良いテストがかけているとどうやって見極めればよいのでしょうか？
自分は誰のためにテストを書いているのかと自分自身に問うてみる。
「誰のためにテストを書けばいいのか？」それは「コードを見る人のため。」
「このコードはどう動くのか」を教えてくれるのが良いテストです。
良いテストの条件
* コンテキスト、出発点、満たすべき条件がわかる。
* ソフトウェアがどのように起動されるかが分かる。
* 期待される結果と、確認すべき事後条件が分かる。

# 91. [良いプログラマになるには](https://プログラマが知るべき97のこと.com/エッセイ/良いプログラマになるには)

[ (英文=> by Pete Goodliffe)](http://programmer.97things.oreilly.com/wiki/index.php/You_Gotta_Care_about_the_Code)
良いコードを書くためには、良いコードを書きたいと心の底から願い、努力した人だけが
本当に良いコードを書けるのです。
良いプログラマーとそうでないプログラマーの違い
それは「取り組む姿勢」
* とりあえず動きそうというプログラムを決して書かない、美しい、シンプルなコードを書く。
コードの正しさを確実に証明できるテストも書く
* わかりやすいコード、保守しやすいコード、正しいコードを書く。
* 他のプログラマーと協調する。他人が読みやすいコードを書く、チーム全体の成果を最良にすることを考える。
* 自分が扱ったコードは、必ず、自分が最初に見た時よりも少しでも良いコードにする。
* 絶えず積極的に新しい言語、イディオム、テクニックを学ぶ。
ただし学んだことをむやみに使わない。適切と判断した場合にのみ使う。
自ら誇りに思えるプログラムを書きましょう。

# 92. [顧客の言葉はそのまま受け取らない](https://プログラマが知るべき97のこと.com/エッセイ/顧客の言葉はそのまま受け取らない)

[ (英文=> by Nate Jackson)](http://programmer.97things.oreilly.com/wiki/index.php/Your_Customers_Do_not_Mean_What_They_Say)
顧客は自分のほしいものがうまく言葉に出来ない。
これは顧客との関わりを密にして解決する。
顧客の言葉をそのまま受け取らない。

# 93. [エラーを無視するな](https://プログラマが知るべき97のこと.com/エッセイ/エラーを無視するな)

[ (英文=> by Pete Goodliffe)](http://programmer.97things.oreilly.com/wiki/index.php/Don%27t_Ignore_that_Error%21)
エラーが起きているのに、大したことはないと思い込もうとする。大丈夫だと
自分に言い聞かせて無視する。そんなことをしても何も良いことはないのです。
問題の存在を察知したら、できるだけ早く対処すべきです。先延ばしは禁物です。

# 94. [リンカは魔法のプログラムではない](https://プログラマが知るべき97のこと.com/エッセイ/リンカは魔法のプログラムではない)

[ (英文=> by Walter Bright)](http://programmer.97things.oreilly.com/wiki/index.php/The_Linker_Is_not_a_Magical_Program)
リンカは実はさほど難しいプログラムではありません。
むしろ単純でわかりやすいプログラムです。
処理自体は簡単だけれども、その結果できるものが複雑で、
詳しく検証するのがなかなか面倒ということなのです。

- [D言語 - Wikipedia](https://ja.wikipedia.org/wiki/D言語)
- [Home - D Programming Language](https://dlang.org/index.html)

# 95. [ペアプログラミングと「フロー」](https://プログラマが知るべき97のこと.com/エッセイ/ペアプログラミングと-フロー)

[ (英文=> by Gudny Hauknes, Ann Katrin Gagnat, and Kari Røssland)](http://programmer.97things.oreilly.com/wiki/index.php/Pair_Program_and_Feel_the_Flow)
ペアプログラミングで大切なことは
自分より経験が浅い場合、忍耐強く接すること。
自分より技術力がある人の場合、気後れすることなく接すること。
自分や他のメンバーの長所や短所がどこにあるのっか、
それを注意深く見るようにしましょう。
* 不慮の事態の影響を最小限に抑えることが出来る。
* 問題解決が容易
* 統合がスムーズ
* 割り込みの影響を緩和できる。
* 新人が早くプロジェクトに馴染む。
フロー状態になれば生産性は驚くほど向上します、
しかしその除隊は簡単に壊れます。
自分をフロー状態にするため、またその状態を維持するために、
あらゆる手段を講じましょう。

- [ペアプログラミング―エンジニアとしての指南書-ローリー-ウィリアムズ](http://amzn.to/2yWbOwJ)
- [Pair Programming Illuminated: Laurie Kessler, Robert Williams](http://amzn.to/2zPReuT)
- [Truck Number](http://wiki.c2.com/?TruckNumber)

# 96. [テストは正確に、具体的に](https://プログラマが知るべき97のこと.com/エッセイ/テストは正確に-具体的に)

[ (英文=> by Kevlin Henney)](http://programmer.97things.oreilly.com/wiki/index.php/Test_Precisely_and_Concretely)

- 番号17、77と同一人物
正確だけでは不十分、誤解の余地のないものにしなくてはならない。

- [February 1981 Table of Contents | Communications of the ACM](https://cacm.acm.org/magazines/1981/2)

# 97. [ステートに注目する](https://プログラマが知るべき97のこと.com/エッセイ/ステートに注目する)

[ (英文=> by Niclas Nilsson)](http://programmer.97things.oreilly.com/wiki/index.php/Thinking_in_States)
ステートは非常に重要です。
具体的にどういう注意をすべきか？
基本は「ステートマシン」という考え方を理解することでしょう。
Stateパターン（デザインパターンにおける23の主要なパターンの一つ）に
ついても学びましょう。
それが十分に理解できたら「契約による設計」などについても学びましょう。
ステートに注目して考えれば、コードをよりシンプルに、
そして堅牢にすることにつながります。

- [オブジェクト指向における再利用のためのデザインパターン-エリック-ガンマ](http://amzn.to/2i2SovC)
- [Design Patterns: Elements of Reusable Object-Oriented Software (Addison-Wesley Professional Computing Series)](http://amzn.to/2i1Lg2x)
- [オブジェクト指向入門-第2版-原則・コンセプト-Architect’Archive-クラシックモダン・コンピューティング](http://amzn.to/2zT3EC2)
- [Object-Oriented Software Construction (Book/CD-ROM) (Prentice-hall International Series in Computer Science) ](http://amzn.to/2yXwLr6)

# 01 (日). [命を吹き込む魔法](https://プログラマが知るべき97のこと.com/エッセイ/命を吹き込む魔法) 森田創

 日本語のみ
プロジェクトにコードネームを付けましょう。
コードネームはチームを結束する秘密の合言葉であり、
プロジェクトを遊ぶための無害な口実であり、
姿の見えないソフトウェアに命を吹き込む魔法なのです。

# 02 (日). [ロールプレイングゲーム](https://プログラマが知るべき97のこと.com/エッセイ/ロールプレイングゲーム) 関将俊

 日本語のみ
ちょっと良いプログラマになるためのコツ
まるで「理想のプログラマ」のように仕事をするための簡単なアイデア。
お仕事中は淡々と理想のプログラマを演じてみましょう。
迷ったら仕事だと諦めて演じてください、だって、仕事でしょ？

# 03 (日). [ルーチンワークをフローのきっかけに](https://プログラマが知るべき97のこと.com/エッセイ/ルーチンワークをフローのきっかけに) 宮川達彦

 日本語のみ
ルーチンワークは自動化しましょう、
ただ、ほんの少しだけ、その作業で手や頭を動かす余地を残しておくのも、
プログラマがクリエティブになる準備としては、悪くないかもしれません。
フロー状態＝周りの様が下がなくコーディングに没頭している状態。

# 04 (日). [プログラマが持つべき3つのスキル](https://プログラマが知るべき97のこと.com/エッセイ/プログラマが持つべき3つのスキル) 吉岡弘隆

 日本語のみ
* コードを読むスキル
* テストをするスキル
* デバッグをするスキル。
これらのスキルは知識の獲得と違って、実際に体を動かし、試行錯誤をし
時には失敗して身につけなければならないのです。
残念ながらこれらのスキル身につけるための体系的に記述した参考書などほとんどありません。
開発の現場で経験を積むしか無いのが現状です。
"「Code Reading オープンソースから学ぶソフトウェア開発技法」
http://amzn.to/2gBb4pw
（高い！）"
どうすればいいのか？
理想は仕事の場で師匠と呼べるような人の下につく。（難しい！）
それではどうするか？
オープンソースソフトウェア（OSS)です。
定番のOSSには支障となるべきカリスマプログラマがいます。
開発メーリングリストを購読すれば、ソフトウェアのバグや新機能の仕様について
議論していることを見聞きできます。
そのなかから自分が興味を持った問題に取り組んでみたらどうでしょうか？
まずは、簡単なバグを一つ選んで試しにデバッグしてみます。
ひょっとしたらすでにそのバグに対するパッチは書かれているかもしれません、
ですが、練習なので気にしません。
実際のバグを直すという練習は、コードを読むスキル、テストをするスキル、
デバッグをするスキルをバランスよく練習できます。

- [Code Reading ~オープンソースから学ぶソフトウェア開発技法~ (プレミアムブックス版) | Diomidis Spinellis, まつもと ゆきひろ, 平林 俊一, 鵜飼 文, トップスタジオ](http://amzn.to/2yWveSl)
- [オープンソースソフトウェアの育て方 | Karl Fogel, 高木 正弘, 高岡 芳成](http://amzn.to/2gUnetV)
- [Producing Open Source Software: How to Run a Successful Free Software Project: Karl Fogel](http://amzn.to/2lsSSjI)

# 05 (日). [快適な環境を追求する](https://プログラマが知るべき97のこと.com/エッセイ/快適な環境を追求する) 舘野祐一

 日本語のみ
ちょっと時間を割いて快適な環境づくりを行うことで、コーディングするための
時間をより快適に過ごすことが出来るようになります。
快適な環境を作ることに貪欲になりましょう。

# 06 (日). [見知らぬ人ともうまくやるには](https://プログラマが知るべき97のこと.com/エッセイ/見知らぬ人ともうまくやるには) 小飼弾

 日本語のみ
バグには2種類ある
出来るはずのことが出来ない。
出来てはならないことが出来てしまう。
プログラマーは前者は特に注意するが、後者はあまり注意を払わないように思われます。
どうすればよいか？
出来てはならぬことを出来なくするには、「出来てはならぬことを禁じる」ではなく、
はじめから「出来ていいことだけを出来るようにする」と考えるのです。
見知らぬ人とうまくやる一番のコツは、見知らぬことをしないこと。

- [lleval - run codes from your browser](http://colabv6.dan.co.jp/lleval.html)
- [codepad](http://codepad.org/)

# 07 (日). [不具合にテストを書いて立ち向かう](https://プログラマが知るべき97のこと.com/エッセイ/不具合にテストを書いて立ち向かう) 和田卓人

 日本語のみ
テスト駆動開発で対応する。
心がけている一つの掟
「不具合の修正時には必ず先に不具合を再現する自動テストを書いてから修正する」
手順
手元で不具合を再現させる
コードを注意深く調べ、不具合を発生させている最小部分を絞り込む。
最小レベルで不具合を再現させ、不具合が修正されたら通るような自動テストコードを書く。
このテストコードを実行し、落ちることを確認する。
不具合を修正する。
テストが通ることを確認する。
既存のすべてのテストを実行し、不具合修正が他の部分を壊していないことを確認する。
メリット
不具合が本当に自分の考えた原因で発生しているかが明らかになる。
対象コードと対象領域に対する理解が深まる。
自分の弱点、気づきにくい点が分かる。
テストの堅牢さ、価値が上がる。

# 08 (日). [育ちのよいコード](https://プログラマが知るべき97のこと.com/エッセイ/育ちのよいコード) 森田創

 日本語のみ
高凝集と疎結合が優れた設計の指標
本当に上手い抽象なのかどうかを視点を変えて考えてみる。
コードのレポジトリをチェックアウトし、それまでチェックインされた変更、パッチを調べます。
そのパッチがひとかたまりの「＋」行から出来ているなら期待が持てそうです。
高凝集なコードなら変更が一箇所にまとまるはずです。
リファクタリングとそれ以外の変更を別のパッチとしてチェックインさせます。
リファクタリングをしないコードに明るい未来はありません。
リファクタリングの原則は振る舞いを変更しない。
読み手が振る舞い自体の正しさを気にしなくてすみます。

# 09 (日). [Noといえることの大事さ](https://プログラマが知るべき97のこと.com/エッセイ/Noといえることの大事さ) 宮川達彦

 日本語のみ
声の大きいユーザーの要求するニッチな機能をどんどん追加してしまった肥大化したソフトウェアを
Feature Creep と呼ばれ、ソフトウェアが破滅に向かう第一歩（あるいは手遅れ）
の状態になります。
この悲劇を避けるためには
そうした要望に「No！」といえる勇気です。
ソフトウェアの本体で実装するのは避けて、拡張機能の形で実装したり、
プラグインのようにコアのコードを変更することなく動作を変更できるようなデザインにする。

# 10 (日). [名前重要](https://プログラマが知るべき97のこと.com/エッセイ/名前重要) まつもとゆきひろ

 日本語のみ
適切な名前をつけられると言うことは、その機能が正しく理解されて、設計されているということで、逆にふさわしい名前がつけられないということは
その機能が果たすべき役割を設計者自身も十分理解できないということ。
適切な名前がつけられれば、その設計の8割が完成したと言ってもいいすぎではない。
ソフトウェア設計のアプローチとして「まず名前から入る」というのは、
あまり語られていない秘訣としてもっと広く知られてもいいように思います。

私の設計上の座右の銘は「名前重要」ｂｙまつもとひろゆき

- - -
## 参考リンク
- [「プログラマが知るべき97のこと」日本語版 ](https://プログラマが知るべき97のこと.com/エッセイ/)
- [「97 Things Every Programmer Should Know」英語版 ](http://programmer.97things.oreilly.com/)

- - -
## License
このページは「[CC-by-3.0-USライセンス](https://creativecommons.org/licenses/by/3.0/us/deed.ja)」に従います。
- https://creativecommons.org/licenses/by/3.0/us/
- https://freedomdefined.org/Licenses/CC-BY-3.0
