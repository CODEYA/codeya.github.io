---
title: 文書記述ガイドライン
permalink: /documents/documentation-guidelines.html
overview:
---

# 概要

本書では CODEYA における文書記述に関するガイドラインを提供する。
本書のステータスは Working Draft であり、本書に対するご意見は pull request にてお送りいただきたい。

## 前提

本書における "MUST"、"MUST NOT"、"SHOULD"、"SHOULD NOT"、"MAY" という表記は [RFC2119](http://www.asahi-net.or.jp/~sd5a-ucd/rfc-j/rfc-2119j.html) における定義に従う。

# 文体

* [常体(である調)](http://ja.wikipedia.org/wiki/%E5%B8%B8%E4%BD%93)を用いる(MUST)。
* [仮名交じり文](http://ja.wikipedia.org/wiki/%E4%BB%AE%E5%90%8D%E4%BA%A4%E3%81%98%E3%82%8A%E6%96%87)を用いる(MUST)。

# 使用可能文字

* [Unicode](http://unicode.org/) に定義されている文字を使用する(MUST)。
* ただし、以下のいずれにも該当しないものは可能な限り使用しない(SHOULD)。
  * [JIS X 0201 ラテン文字用図形文字集合](http://ja.wikipedia.org/wiki/JIS_X_0201#.E3.83.A9.E3.83.86.E3.83.B3.E6.96.87.E5.AD.97.E7.94.A8.E5.9B.B3.E5.BD.A2.E6.96.87.E5.AD.97.E9.9B.86.E5.90.88) に含まれる文字
  * [JIS X 0208](http://ja.wikipedia.org/wiki/JIS_X_0208) に含まれる文字
* 数字、記号は可能な限り[JIS X 0201 ラテン文字用図形文字集合](http://ja.wikipedia.org/wiki/JIS_X_0201#.E3.83.A9.E3.83.86.E3.83.B3.E6.96.87.E5.AD.97.E7.94.A8.E5.9B.B3.E5.BD.A2.E6.96.87.E5.AD.97.E9.9B.86.E5.90.88)のものを用いる(SHOULD)。
* [約物](http://ja.wikipedia.org/wiki/%E7%B4%84%E7%89%A9)は全角記号を使用する。句点として "。"、読点として"、"を使用する(MUST)。

# 可読性

* 接続詞や接続助詞を用いて文章を接続することを避け、短く簡潔に記述する(SHOULD)。
* 無駄な形容詞、副詞の利用をさける(SHOULD)。

# 数字

数字はアラビア数字を用いる(MUST)。
ただし、以下においては漢数字を用いる(MUST)。

1. 固有名詞
```
(例) 三田　九州
```
2. 概数
```
(例) 数十件　数百人
```
3. 単語の一部、慣用表現
```
(例) 四捨五入　一般　二日酔い　一休み
```

# 漢字

『[常用漢字(平成22年内閣告示第2号)](http://www.bunka.go.jp/kokugo_nihongo/kokujikunrei_h221130.html)』に従う(MUST)。

ただし、以下に該当する語については常用漢字によって記載可能であってもかな書きとする(MUST)。

```
かつ(且つ)　また(又)　ただし(但し)　もし(若し)　ほか(他、外)　しかし(然し)　したがって(従って)　なお(尚)
ならびに(並びに)　それ(其れ)　いつ(何時)　どこ(何処)　なぜ(何故)　ある(有る)　ない(無い)　できる(出来る)
なる(成る)　いる(居る)　こと(事)　ごと(毎)　もの(物)　など(等)　よう(様)　くらい(位)　ため(為)　とき(時)　
ところ(所)　ほど(程)　はず(筈)　まで(迄)　もって(以て)
```

# 仮名遣い

『[現代仮名遣い(平成22年内閣告示第4号)](http://kokugo.bunka.go.jp/kokugo_nihongo/joho/kijun/naikaku/gendaikana/index.html)』 に従う(MUST)。

# 送り仮名

『[送り仮名の付け方(平成22年内閣告示第3号)](http://kokugo.bunka.go.jp/kokugo_nihongo/joho/kijun/naikaku/okurikana/index.html)』に従う(MUST)。

## 『送り仮名の付け方(平成22年内閣告示第3号)』(転載)
### 単独の語

#### 1 活用のある語

##### 通則1

**本則**
活用のある語(通則2を適用する語を除く。)は，活用語尾を送る。

```
〔例〕　
憤る　承る　書く　実る　催す
生きる　陥れる　考える　助ける
荒い　潔い　賢い　濃い
主だ
```

**例外**

(1)　語幹が「し」で終わる形容詞は，「し」から送る。

```
〔例〕　
著しい　惜しい　悔しい　恋しい　珍しい
```

(2)　活用語尾の前に「か」，「やか」，「らか」を含む形容動詞は，その音節から送る。

```
〔例〕　
暖かだ　細かだ　静かだ
穏やかだ　健やかだ　和やかだ
明らかだ　平らかだ　滑らかだ　柔らかだ
```

(3)　次の語は，次に示すように送る。

```
明らむ　味わう　哀れむ　慈しむ　教わる　脅かす(おどかす)　脅かす(おびやかす)　食らう　異なる　逆らう　捕まる　群がる　和らぐ　揺する
明るい　危ない　危うい　大きい　少ない　小さい　冷たい　平たい
新ただ　同じだ　盛んだ　平らだ　懇ろだ　惨めだ
哀れだ　幸いだ　幸せだ　巧みだ
```

許容　次の語は，(　)の中に示すように，活用語尾の前の音節から送ることができる。
表す(表わす)　著す(著わす)　現れる(現われる)　行う(行なう)　断る(断わる)　賜る(賜わる)
(注意)　語幹と活用語尾との区別がつかない動詞は，例えば，「着る」，「寝る」，「来る」などのように送る。

##### 通則2

**本則**　
活用語尾以外の部分に他の語を含む語は，含まれている語の送り仮名の付け方によって送る。(含まれている語を〔　〕の中に示す。)

(1)　動詞の活用形又はそれに準ずるものを含むもの。

```
〔例〕
動かす〔動く〕　照らす〔照る〕
語らう〔語る〕　計らう〔計る〕　向かう〔向く〕
浮かぶ〔浮く〕
生まれる〔生む〕　押さえる〔押す〕　捕らえる〔捕る〕
勇ましい〔勇む〕　輝かしい〔輝く〕　喜ばしい〔喜ぶ〕
晴れやかだ〔晴れる〕
及ぼす〔及ぶ〕　積もる〔積む〕　聞こえる〔聞く〕
頼もしい〔頼む〕
起こる〔起きる〕　落とす〔落ちる〕
暮らす〔暮れる〕　冷やす〔冷える〕
当たる〔当てる〕　終わる〔終える〕　変わる〔変える〕　　集まる〔集める〕　定まる〔定める〕　連なる〔連ねる〕　交わる〔交える〕
混ざる・混じる〔混ぜる〕
恐ろしい〔恐れる〕
```

(2)　形容詞・形容動詞の語幹を含むもの。

```
〔例〕
重んずる〔重い〕　若やぐ〔若い〕
怪しむ〔怪しい〕　悲しむ〔悲しい〕　苦しがる〔苦しい〕
確かめる〔確かだ〕
重たい〔重い〕　憎らしい〔憎い〕　古めかしい〔古い〕
細かい〔細かだ〕　柔らかい〔柔らかだ〕
清らかだ〔清い〕　高らかだ〔高い〕　寂しげだ〔寂しい〕
```

(3)　名詞を含むもの。

```
〔例〕
汗ばむ〔汗〕　先んずる〔先〕　春めく〔春〕
男らしい〔男〕　後ろめたい〔後ろ〕
```

許容　読み間違えるおそれのない場合は，活用語尾以外の部分について，次の(　)の中に示すように，送り仮名を省くことができる。

```
〔例〕　
浮かぶ(浮ぶ)　生まれる(生れる)　押さえる(押える)　捕らえる(捕える)
晴れやかだ(晴やかだ)
積もる(積る)　聞こえる(聞える)
起こる(起る)　落とす(落す)　暮らす(暮す)　当たる(当る)　終わる(終る)　変わる(変る)
(注意)　次の語は，それぞれ〔　〕の中に示す語を含むものとは考えず，通則1によるものとする。
明るい〔明ける〕　荒い〔荒れる〕　悔しい〔悔いる〕　恋しい〔恋う〕
```

#### 2 活用のない語

##### 通則3

**本則**
名詞(通則4を適用する語を除く。)は，送り仮名を付けない。

```
〔例〕　
月　鳥　花　山
男　女
彼　何
```

**例外**

(1)　次の語は，最後の音節を送る。

```
辺り　哀れ　勢い　幾ら　後ろ　傍ら　幸い　幸せ　互い　便り　半ば　情け　斜め　独り　誉れ　自ら　災い
```

(2)　数をかぞえる「つ」を含む名詞は，その「つ」を送る。

```
〔例〕　
一つ　二つ　三つ　幾つ
```

##### 通則4

**本則**　
活用のある語から転じた名詞及び活用のある語に「さ」，「み」，「げ」などの接尾語が付いて名詞になったものは，もとの語の送り仮名の付け方によって送る。

(1)　活用のある語から転じたもの。

```
〔例〕
動き　仰せ　恐れ　薫り　曇り　調べ　届け　願い　晴れ
当たり　代わり　向かい
狩り　答え　問い　祭り　群れ
憩い　愁い　憂い　香り　極み　初め
近く　遠く
```

(2)　「さ」，「み」，「げ」などの接尾語が付いたもの。

```
〔例〕
暑さ　大きさ　正しさ　確かさ
明るみ　重み　憎しみ
惜しげ
```

**例外**　
次の語は，送り仮名を付けない。

```
謡　虞　趣　氷　印　　頂　帯　畳
卸　煙　恋　志　次　隣　富　恥　話　光　舞
折　係　掛(かかり)　組　肥　並(なみ)　巻　割
```

(注意)　ここに掲げた「組」は，「花の組」，「赤の組」などのように使った場合の「くみ」であり，例えば，「活字の組みがゆるむ。」などとして使う場合の「くみ」を意味するものではない。「光」，「折」，「係」なども，同様に動詞の意識が残っているような使い方の場合は，この例外に該当しない。したがって，本則を適用して送り仮名を付ける。
許容　読み間違えるおそれのない場合は，次の(　)の中に示すように，送り仮名を省くことができる。

```
〔例〕　
曇り(曇)　届け(届)　願い(願)　晴れ(晴)
当たり(当り)　代わり(代り)　向かい(向い)
狩り(狩)　答え(答)　問い(問)　祭り(祭)　群れ(群)
憩い(憩)
```

##### 通則5

**本則**
副詞・連体詞・接続詞は，最後の音節を送る。

```
〔例〕　
必ず　更に　少し　既に　再び　全く　最も
来る　去る
及び　且つ　但し
```

**例外**　

(1)　次の語は，次に示すように送る。

```
明くる　大いに　直ちに　並びに　若しくは
```

(2)　次の語は，送り仮名を付けない。

又

(3)　次のように，他の語を含む語は，含まれている語の送り仮名の付け方によって送る。(含まれている語を〔　〕の中に示す。)

```
〔例〕　
併せて〔併せる〕　至って〔至る〕　恐らく〔恐れる〕　従って〔従う〕　絶えず〔絶える〕　例えば〔例える〕　努めて〔努める〕
辛うじて〔辛い〕　少なくとも〔少ない〕
互いに〔互い〕
必ずしも〔必ず〕
```

### 複合の語

##### 通則6

**本則**
複合の語(通則7を適用する語を除く。)の送り仮名は，その複合の語を書き表す漢字の，それぞれの音訓を用いた単独の語の送り仮名の付け方による。

(1)　活用のある語

```
〔例〕
書き抜く　流れ込む　申し込む　　打ち合わせる　向かい合わせる　長引く　若返る　　裏切る　旅立つ
聞き苦しい　　薄暗い　　草深い　心細い　　待ち遠しい　　軽々しい　若々しい　女々しい
気軽だ　　望み薄だ
```

(2)　活用のない語

```
〔例〕
石橋　竹馬　山津波　　後ろ姿　斜め左　花便り　独り言　　卸商
水煙　目印
田植え　封切り　物知り　落書き　雨上がり　　墓参り　日当たり
夜明かし　先駆け　巣立ち　手渡し
入り江　飛び火　教え子　合わせ鏡　生き物　落ち葉　預かり金
寒空　深情け
愚か者
行き帰り　伸び縮み　乗り降り　　抜け駆け　作り笑い　暮らし向き　　売り上げ　取り扱い　乗り換え　引き換え　　歩み寄り　申し込み　移り変わり
長生き　早起き　苦し紛れ　　大写し
粘り強さ　有り難み　待ち遠しさ
乳飲み子　無理強い　　立ち居振る舞い　呼び出し電話
次々　常々
近々　深々
休み休み　行く行く
```

許容　読み間違えるおそれのない場合は，次の(　)の中に示すように，送り仮名を省くことができる。

```
〔例〕　
書き抜く(書抜く)　申し込む(申込む)　打ち合わせる(打ち合せる・打合せる)　向かい合わせる(向い合せる)　聞き苦しい(聞苦しい)　待ち遠しい(待遠しい)
田植え(田植)　封切り(封切)　落書き(落書)　雨上がり(雨上り)　日当たり(日当り)　夜明かし(夜明し)
入り江(入江)　飛び火(飛火)　合わせ鏡(合せ鏡)　預かり金(預り金)
抜け駆け(抜駆け)　暮らし向き(暮し向き)　売り上げ(売上げ・売上)　取り扱い(取扱い・取扱)　乗り換え(乗換え・乗換)　引き換え(引換え・引換)　申し込み(申込み・申込)　移り変わり(移り変り)
有り難み(有難み)　待ち遠しさ(待遠しさ)
立ち居振る舞い(立ち居振舞い・立ち居振舞・立居振舞)　呼び出し電話(呼出し電話・呼出電話)
```

(注意)　「こけら落とし(こけら落し)」，「さび止め」，「洗いざらし」，「打ちひも」のように，前又は後ろの部分を仮名で書く場合は，他の部分については，単独の語の送り仮名の付け方による。

##### 通則7

複合の語のうち，次のような名詞は，慣用に従って，送り仮名を付けない。

(１)　特定の領域の語で，慣用が固定していると認められるもの。

ア　地位・身分・役職等の名。

```
〔例〕
関取　頭取　取締役　事務取扱
```

イ　工芸品の名に用いられた「織」，「染」，「塗」等。

```
〔例〕
((博多))織　((型絵))染　((春慶))塗　((鎌倉))彫　((備前))焼
```

ウ　その他。

```
〔例〕
書留　気付　切手　消印　小包　振替　　切符　踏切
請負　売値　買値　仲買　歩合　両替　割引　　組合　手当
倉敷料　作付面積
売上((高))　貸付((金))　借入((金))　繰越((金))　小売((商))　積立((金))　取扱((所))　取扱((注意))　取次((店))　取引((所))　乗換((駅))　乗組((員))　引受((人))　引受((時刻))　引換((券))　((代金))引換　振出((人))　待合((室))　見積((書))　申込((書))
```

(２)　一般に，慣用が固定していると認められるもの。

```
〔例〕
奥書　木立　子守　献立　座敷　試合　字引　場合　羽織　葉巻　番組　番付　日付　水引　物置　物語　役割　屋敷　夕立　割合
合図　合間　植木　置物　織物　貸家　敷石　敷地　敷物　立場　建物　並木　巻紙　受付　受取
浮世絵　絵巻物　仕立屋
```

(注意)

(1)　「((博多))織」，「売上((高))」などのようにして掲げたものは，((　))の中を他の漢字で置き換えた場合にも，この通則を適用する。

(2)　通則7を適用する語は，例として挙げたものだけで尽くしてはいない。したがって，慣用が固定していると認められる限り，類推して同類の語にも及ぼすものである。通則7を適用してよいかどうか判断し難い場合には，通則6を適用する。

### 付表の語

「常用漢字表」の「付表」に掲げてある語のうち，送り仮名の付け方が問題となる次の語は，次のようにする。

１　次の語は，次に示すように送る。

```
浮つく　お巡りさん　差し支える　五月晴れ　立ち退く　手伝う　最寄り
なお，次の語は，(　)の中に示すように，送り仮名を省くことができる。
差し支える(差支える)　五月晴れ(五月晴)　立ち退く(立退く)
```

２　次の語は，送り仮名を付けない。

```
息吹　桟敷　時雨　築山　名残　雪崩　吹雪　迷子　行方
```

# カタカナ語表記

『[外来語の表記(平成3年内閣告示第二号)](http://kokugo.bunka.go.jp/kokugo_nihongo/joho/kijun/naikaku/gairai/index.html)』に従う(MUST)。

## 『外来語の表記(平成3年内閣告示第二号)』(転載、部分抜粋)

### 「外来語の表記」に用いる仮名と符号の表

1. 第1表に示す仮名は，外来語や外国の地名・人名を書き表すのに一般的に用いる仮名とする。
2. 第2表に示す仮名は，外来語や外国の地名・人名を原音や原つづりになるべく近く書き表そうとする場合に用いる仮名とする。
3. 第1表・第2表に示す仮名では書き表せないような，特別な音の書き表し方については，ここでは取決めを行わず，自由とする。
4. 第1表・第2表によって語を書き表す場合には，おおむね留意事項を適用する。

<table border="1" cellpadding="0" cellspacing="0">
<tbody><tr>
<td colspan="10"><p>第1表</p></td>
</tr>
<tr>
<td><p>ア</p></td>
<td><p>イ</p></td>
<td><p>ウ</p></td>
<td><p>エ</p></td>
<td><p>オ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
</tr>
<tr>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>シェ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
</tr>
<tr>
<td><p>カ</p></td>
<td><p>キ</p></td>
<td><p>ク</p></td>
<td><p>ケ</p></td>
<td><p>コ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
</tr>
<tr>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>チェ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
</tr>
<tr>
<td><p>サ</p></td>
<td><p>シ</p></td>
<td><p>ス</p></td>
<td><p>セ</p></td>
<td><p>ソ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
</tr>
<tr>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>ツァ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>ツェ</p></td>
<td><p>ツォ</p></td>
</tr>
<tr>
<td><p>タ</p></td>
<td><p>チ</p></td>
<td><p>ツ</p></td>
<td><p>テ</p></td>
<td><p>ト</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
</tr>
<tr>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>ティ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
</tr>
<tr>
<td><p>ナ</p></td>
<td><p>ニ</p></td>
<td><p>ヌ</p></td>
<td><p>ネ</p></td>
<td><p>ノ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
</tr>
<tr>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>ファ</p></td>
<td><p>フィ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>フェ</p></td>
<td><p>フォ</p></td>
</tr>
<tr>
<td><p>ハ</p></td>
<td><p>ヒ</p></td>
<td><p>フ</p></td>
<td><p>ヘ</p></td>
<td><p>ホ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
</tr>
<tr>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>ジェ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
</tr>
<tr>
<td><p>マ</p></td>
<td><p>ミ</p></td>
<td><p>ム</p></td>
<td><p>メ</p></td>
<td><p>モ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
</tr>
<tr>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>ディ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
</tr>
<tr>
<td><p>ヤ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>ユ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>ヨ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
</tr>
<tr>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>デュ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
</tr>
<tr>
<td><p>ラ</p></td>
<td><p>リ</p></td>
<td><p>ル</p></td>
<td><p>レ</p></td>
<td><p>ロ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
</tr>
<tr>
<td><p>ワ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
</tr>
<tr>
<td><p>ガ</p></td>
<td><p>ギ</p></td>
<td><p>グ</p></td>
<td><p>ゲ</p></td>
<td><p>ゴ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
</tr>
<tr>
<td><p>ザ</p></td>
<td><p>ジ</p></td>
<td><p>ズ</p></td>
<td><p>ゼ</p></td>
<td><p>ゾ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
</tr>
<tr>
<td><p>ダ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>デ</p></td>
<td><p>ド</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
</tr>
<tr>
<td><p>バ</p></td>
<td><p>ビ</p></td>
<td><p>ブ</p></td>
<td><p>ベ</p></td>
<td><p>ボ</p></td>
<td colspan="5"><p>第2表</p></td>
</tr>
<tr>
<td><p>パ</p></td>
<td><p>ピ</p></td>
<td><p>プ</p></td>
<td><p>ペ</p></td>
<td><p>ポ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
</tr>
<tr>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>イェ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
</tr>
<tr>
<td><p>キャ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>キュ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>キョ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
</tr>
<tr>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>ウィ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>ウェ</p></td>
<td><p>ウォ</p></td>
</tr>
<tr>
<td><p>シャ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>シュ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>ショ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
</tr>
<tr>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>クァ</p></td>
<td><p>クィ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>クェ</p></td>
<td><p>クォ</p></td>
</tr>
<tr>
<td><p>チャ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>チュ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>チョ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
</tr>
<tr>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>ツィ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
</tr>
<tr>
<td><p>ニャ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>ニュ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>ニョ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
</tr>
<tr>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>トゥ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
</tr>
<tr>
<td><p>ヒャ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>ヒュ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>ヒョ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
</tr>
<tr>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>グァ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
</tr>
<tr>
<td><p>ミャ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>ミュ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>ミョ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
</tr>
<tr>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>ドゥ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
</tr>
<tr>
<td><p>リャ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>リュ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>リョ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
</tr>
<tr>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>ヴァ</p></td>
<td><p>ヴィ</p></td>
<td><p>ヴ</p></td>
<td><p>ヴェ</p></td>
<td><p>ヴォ</p></td>
</tr>
<tr>
<td><p>ギャ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>ギュ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>ギョ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
</tr>
<tr>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>テュ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
</tr>
<tr>
<td><p>ジャ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>ジュ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>ジョ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
</tr>
<tr>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>フュ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
</tr>
<tr>
<td><p>ビャ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>ビュ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>ビョ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
</tr>
<tr>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>ヴュ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
</tr>
<tr>
<td><p>ピャ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>ピュ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>ピョ</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
</tr>
<tr>
<td colspan="5"><p>ン(撥音)</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
</tr>
<tr>
<td colspan="5"><p>ッ(促音)</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
</tr>
<tr>
<td colspan="5"><p>ー(長音符号)</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
<td><p>&nbsp;&nbsp;</p></td>
</tr>
</tbody></table>

### 留意事項その1(原則的な事項)

3. 語形やその書き表し方については，慣用が定まっているものはそれによる。分野によって異なる慣用が定まっている場合には，それぞれの慣用によって差し支えない。

4. 国語化の程度の高い語は，おおむね第1表に示す仮名で書き表すことができる。一方，国語化の程度がそれほど高くない語，ある程度外国語に近く書き表す必要のある語――特に地名・人名の場合――は，第2表に示す仮名を用いて書き表すことができる。

5. 第2表に示す仮名を用いる必要がない場合は，第1表に示す仮名の範囲で書き表すことができる。
例　イェ→イエ　ウォ→ウオ　トゥ→ツ，ト　ヴァ→バ

6. 特別な音の書き表し方については，取決めを行わず，自由とすることとしたが，その中には，例えば，「スィ」「ズィ」「グィ」「グェ」「グォ」「キェ」「ニェ」「ヒェ」「フョ」「ヴョ」等の仮名が含まれる。

### 留意事項その2(細則的な事項)

#### [Roman3 ]　撥音，促音，長音その他に関するもの

1. 撥音は，「ン」を用いて書く。

```
〔例〕　コンマ　シャンソン　トランク　メンバー　ランニング　ランプ
ロンドン(地)　レンブラント(人)
```

注1　撥音を入れない慣用のある場合は，それによる。

```
〔例〕　イニング(←インニング)　サマータイム(←サンマータイム)
```

注2　「シンポジウム」を「シムポジウム」と書くような慣用もある。

2. 促音は，小書きの「ッ」を用いて書く。

```
〔例〕　カップ　シャッター　リュックサック　ロッテルダム(地)　バッハ(人)
```

注　促音を入れない慣用のある場合は，それによる。

```
〔例〕　アクセサリー(←アクセッサリー)　フィリピン(地)(←フィリッピン)
```

3. 長音は，原則として長音符号「ー」を用いて書く。

```
〔例〕　エネルギー　オーバーコート　グループ　ゲーム　ショー　テーブル　パーティー　ウェールズ(地)　ポーランド(地)　ローマ(地)　ゲーテ(人)　ニュートン(人)
```

注1　長音符号の代わりに母音字を添えて書く慣用もある。

```
〔例〕　バレエ(舞踊)　ミイラ
```

注2　「エー」「オー」と書かず，「エイ」「オウ」と書くような慣用のある場合は，それによる。

```
〔例〕　エイト　ペイント　レイアウト　スペイン(地)　ケインズ(人)　サラダボウル　ボウリング(球技)
```

注3　英語の語末の‐er,　‐or,　‐arなどに当たるものは，原則としてア列の長音とし長音符号「ー」を用いて書き表す。ただし，慣用に応じて「ー」を省くことができる。

```
〔例〕　エレベーター　ギター　コンピューター　マフラー
エレベータ　コンピュータ　スリッパ
```

4. イ列・エ列の音の次のアの音に当たるものは，原則として「ア」と書く。

```
〔例〕　グラビア　ピアノ　フェアプレー　アジア(地)　イタリア(地)　ミネアポリス(地)
```

注1　「ヤ」と書く慣用のある場合は，それによる。

```
〔例〕　タイヤ　ダイヤモンド　ダイヤル　ベニヤ板
```

注2　「ギリシャ」「ペルシャ」について「ギリシア」「ペルシア」と書く慣用もある。

5. 語末(特に元素名等)の‐(i)umに当たるものは，原則として「―(イ)ウム」と書く。

```
〔例〕　アルミニウム　カルシウム　ナトリウム　ラジウム
サナトリウム　シンポジウム　プラネタリウム
```

注　「アルミニウム」を「アルミニューム」と書くような慣用もある。

6. 英語のつづりのxに当たるものを「クサ」「クシ」「クス」「クソ」と書くか，「キサ」「キシ」「キス」「キソ」と書くかは，慣用に従う。

```
〔例〕　タクシー　ボクシング　ワックス　オックスフォード(地)
エキストラ　タキシード　ミキサー　テキサス(地)
```

7. 拗音に用いる「ヤ」「ユ」「ヨ」は小書きにする。また，「ヴァ」「ヴィ」「ヴェ」「ヴォ」や「トゥ」のように組み合せて用いる場合の「ア」「イ」「ウ」「エ」「オ」も，小書きにする。


8. 複合した語であることを示すための，つなぎの符号の用い方については，それぞれの分野の慣用に従うものとし，ここでは取決めを行わない。

```
〔例〕　ケースバイケース　ケース・バイ・ケース　ケース―バイ―ケース
マルコ・ポーロ　マルコ=ポーロ
```

# カタカナ表記と英語表記の使い分け

外来語はカタカナ表記を用いる(MUST)。

```
〔例〕タスク　レビュー　コード　スタイル　レイアウト　モジュール　ロジック　デザイン　リソース
```

ただし、以下に該当する語は英語表記とする(MUST)。

1. 固有名詞(仕様名、団体名、ソフトウェア名など)

```
〔例〕JavaScript　Apache　Tomcat　Springframework
```

2. 特定の仕様にて予約語として扱われる語

```
〔例〕public　instanceof　super　volatile
```

ただし、慣用が固定していると認められるものはそれに従う。

```
〔例〕クラス　インターフェース　メソッド　フィールド　プロパティー　オブジェクト　インスタンス
```

3. 特定の技術要素(パッケージ名、モジュール名、クラス名、ファイル名、タグ名、属性名など)を表す語

```
〔例〕StringBuilder　InputStream　Exception　log4j.xml　ApplicationContext　div
```

4. 頭字語

```
〔例〕URL　RAID　TLD　UCS
```

TBD: カタカナ表記と英語表記の使い分けについては、ドキュメントの記載を進めながら再検討が必要。

# メタ記法

| 目的             | 記号                                | 解説                                                                                                        | 備考 |
|------------------|-------------------------------------|-------------------------------------------------------------------------------------------------------------|------|
| リソース参照     | ふたえかぎ 『』                     | リソースの名称、ファイル名、IDを表す。                                                                      |      |
| キーワード参照   | ひとえかぎ 「」                     | キーワードの名称、IDを表す。例えば同一ドキュメント内で定義された項目を他の箇所から参照する際などに利用する。| ひとえかぎは全角を用いる(MUST) |
| ID参照           | アンパーサンド &                    | ID を表す。通常キーワード参照内で利用する。例) 「ユーザー氏名 &ID001」                                      | アンパーサンドは半角を用いる(MUST)  |
| リテラル         | ストレートクォーテーションマーク "" | リテラルを表す。固定値を文章中に記載する際に利用する。例) "MALE"、"FEMALE"                                  | ストレートクォーテーションマークは半角を用いる(MUST) |
| アノーテーション |  アットマーク @                     | アノーテーションを表す。ID に対し、制御用の注釈情報を付与する際に利用する。 例) "@generated"                | アットマークは半角を用いる(MUST) |
| 列挙             | スラッシュ /                        | キーワード、リテラルを列挙する際に利用する。例) "TRUE" / "FALSE"                                            | スラッシュは半角を用いる(MUST) |
| 変数             | ドル記号 $                          | 変数を表す。主に数式内で変数を記述する際に利用する。                         | ドル記号は半角を用いる(MUST) |
