## unittest

https://qiita.com/aomidro/items/3e3449fde924893f18ca

### 使い方

基本的な使い方は以下のとおり。
1. unittestをインポートする
2. unittest.TestCaseを継承したクラスTestHOGEHOGEを作る
3. TestHOGEHOGEの中に、テストケースを記述する。テストケースは、AssetHOGE()という名称の一群のメソッドを使う。このメソッドによって一致・大小関係などなどの比較が行われる。
4. unittest.main()でテストを実行する。所望の通りの結果が実現されていれば、成功、そうでなければ失敗という結果が得られる。

## Advanced Game-playing

⚠depth searchの計算量が膨大という問題がある。

### iterative deep pening

http://movingai.com/dfid.html
動画の通り探索の方法が異なる。

### Understanding Exponential Time

layer levelが増える度に大きな計算量が発生する

### Quiz: Exponential B=3

iterative deepening is visited nodes of numbers.

[![https://diveintocode.gyazo.com/6577a7fd4db6cd5f33331b1f10ed1eec](https://t.gyazo.com/teams/diveintocode/6577a7fd4db6cd5f33331b1f10ed1eec.png)](https://diveintocode.gyazo.com/6577a7fd4db6cd5f33331b1f10ed1eec)


### Varying The Branching Factor

探索するブランチが多すぎるので、2秒で計算することが難しい
そこで、探索するブランチを絞り込む

### ??Horizon Effect

[![https://diveintocode.gyazo.com/1ff43aa7f1c8b779ad849e7991b5465c](https://t.gyazo.com/teams/diveintocode/1ff43aa7f1c8b779ad849e7991b5465c.png)](https://diveintocode.gyazo.com/1ff43aa7f1c8b779ad849e7991b5465c)

自分が動けるところを制限、可視化する？？

### Horizon Effect (Contd.)

### Quiz: Good Evaluation Functions


### The Alpha Beta Search Algorithm

minimaxと比べて探索量を減らすことができる

最適が2であるので、左のブランチが2であればそれ以上探索しない
⚠実際にすべて探索した場合と異なる結果が返ってくるが、

----

`for heuristic function`

### Evaluation Function Intro
単純にコンピュータプレイヤーが動くことができる数で評価する

### Quiz: Testing The Evaluation Function

my_moves

### Testing Evaluation Functions

level3からlevel2にする

### Quiescent Search
levelを変更するだけで結果が変わる
