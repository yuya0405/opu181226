# opu181226

### 提出締め切り
2019年01月23日の14:30まで

### 学籍番号
2170104021

### 氏名
大林 由弥

## 1: 大喜利
```
1, <A>:こんな忍者は嫌だ
2, <B>:[飛び道具]が[ショットガン]
3, <B>:[安全基準]が[宇宙服]
4, <A>:装備が現代的
```
## 2: こんな桃太郎は嫌だ
```
1, <A>:おじいさんとおばあさんがセレブ
2, <A>:吉備団子の代わりが[キットカット]
3, <A>:お供が[スヌーピー]
4, <A>:お供が[リラックマ]
```
## 3: 失ったもの
```
1, <A>:今の私と[学部]の頃の私の違いは何だろう？
2, <A>:せや！word2vecに教えてもらおう！
3, <A>:修士課程マイナス学士は・・・
4, <B>:word2vec「[青春ストーリー]」
```
### リポジトリについて
- 種類：プライベートリポジトリ
  - word2vecのリポジトリ：https://github.com/kd21/simple_word2vec
  - 上のリポジトリを「fork」するという指定であったが，forkしたものはプライベートリポジトリにすることはできない為，新規作成した．
- URL：https://github.com/yuya0405/opu181226

### ソースコードの場所
opu181226/make_wiki_word2vec_for_lec.ipynb

### 補足
- １話目
  - 大喜利の形式にするとボケやすい
  - 「"名詞"が"名詞"」の形がword2vecのライブラリを用いるに当たって使用しやすい文構造
- ２話目
  - word2vecのライブラリで固有名詞・キャラクタ名・有名人の名前を引き当てれば比較的話を組み立てやすい
- ３話目
  - メタ的な構造

### 使用しなかったもの
MeCabを利用して形態素解析を用いることを検討したが，4コマ分の意味の通るテキストを生成する目処が立たなかったので断念した．
- MeCabを利用する方針しては，以下の参考URLにある通り，大喜利における丁度良いボケのパターンに各々品詞を当てはめてオチ等を生成することが挙げられる．
- MeCabは結局のところ使用しなかったものの，自分で手動で書くに当たって以下の文章の組み立て方は意識した．
- 参考：http://bugrammer.hateblo.jp/entry/2015/04/25/140930
```
boke_pattern = [
    [u"名詞"],
    [u"名詞", u"名詞"],
    [u"名詞", u"が", u"名詞"],
    [u"名詞", u"が", u"動詞"],
    [u"名詞", u"が", u"名詞", u"な", u"名詞"],
    [u"名詞", u"が", u"名詞", u"助詞", u"動詞"],
]
```
