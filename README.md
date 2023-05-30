# シン！こうかとん無双改
## 実行環境の必要条件
* python >= 3.10
* pygame >= 2.1

## ゲームの概要
主人公キャラクターは、こうかとんで、矢印キーとスペースキーを押しながら、敵と争うゲーム
プロジェクト演習の第4回の授業でグループで作成したソースコードにメニュー、難易度選択、音楽など、新しい機能を追加したゲーム

## ゲームの実装
###　共通基本機能
* 第4回の授業のソースコード
### 操作方法について
* 矢印キー：こうかとん移動
* スペースキー：敵機に撃つ
* 左Shiftキー：ずっと押してると、こうかとんピートが上がる
* 右Shiftキー：無敵こうかとんになる（スコアが１００点以上の場合）
* CapsLockキー：こうかとんの前に防護壁を生成する（スコアが５０点以上の場合）
### クリア条件について
* 負けまでスコアを取得する
### 追加機能
- タイシア
    * ゲームのメニューを作り
    * メニューで難易度を選択できる
    * メニューでゲームを終了できる
-　大野
    * ビームを放った時に効果音を鳴らす
    * 爆破したときに効果音を鳴らす
    * ゲームオーバーの時に効果音を鳴らす
    * ゲームオーバー時の「GameOver」を表示し、得点も表示する
- 山中
    - こうかとんの残機機能
        * 難易度による残機の変化
        * 効果トンのレベルによる残基回復
- チェヨン
    - ハイスコアが更新されたときに表示
- 吉野
    - ゲームのレベルアップ
    
### 担当以外追加した機能
* メニューで選択した難易度によるEasy、NormalとHard、難しさが違う三つのレベル
* 難易度ではなく、時間とともに難しくなるArcadeレベル
* 負けの時にGame Overメッセージを表示

### ToDo
* 自分が担当していることを全て終えた

### メモ
* 各レベルの内容は、難易度の変数difficultyによる設定する。
* SE_load関数に第一引数にどこの部分の効果音beam,explosion,gameoverのいずれかを与えてあげるとBGMを流すことができる。
* 効果音が流れるのは、ビームを放った時、爆発したとき、ゲームオーバーの時の3つである。
* 点数をhighscore.txtに保存する
* Score クラスに表示するテキストを一部変更
* ハイスコアかを判定して表示させる部分はmain()内に記述
* レベルに応じてゲームの内容が変化するようにしたい
* 他の追加機能との連携が取れたらいいなと思っています

### 参考文献
1. https://www.pygame.org/docs/ Pygameドキュメント
2. https://nosuke.net/archives/729
3. http://westplain.sakura.ne.jp/translate/pygame/ **Pygameドキュメント 日本語訳**
4. https://goodlucknetlife.com/python-shooting-bgm-se/ **シューティングゲームにおけるBGMとSEの実装例【Pygame】**
5. https://shizenkarasuzon.hatenablog.com/entry/2018/12/29/203344 **【Pygame】Pygameでテキストを描画する**
6. http://www.s12600.net/psy/python/02-2.html **効果音とBGMを複数鳴らす**
7. https://nosuke.net/archives/729