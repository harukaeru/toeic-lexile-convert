# TOEICのスコアをlexile指数に換算するやつ

ここにアクセスして、TOEICのリーディングスコアを入力すると出ます。

https://cdn.rawgit.com/harukaeru/toeic-lexile-convert/master/lexile.html

# どういうやつなのか？

http://lerg.lexile.com/ja/

が死んでいて動かないので、再構築した。

元データが幸いにも

http://wayback.archive.org/web/20150320192025/http://lerg.lexile.com/ja

に残っていたのだが、
スクリプトが動いてなかったので、ソース読んでロジックだけ抜き取って簡易化した

ソースが汚くて改変したくなったが、めんどくさかったし、我慢してそのまま使用している(´・ω・｀)

換算が信用できない方はこちらもご覧ください。

http://wayback.archive.org/web/20140820120644/http://square.toeic.or.jp/kyouzai/lexile/about/


動作しない場合は

https://twitter.com/d24d30033e5c469

までリプライかなにかをください

# 所感
TOEIC公式からもサイトがlexile指数に関するものが消えているので、あまり換算はあてにならないかもしれません。

それから`自分のlexile指数 - 250`のレベルのものは90%、自分のlexile指数と同じ指数のレベルの文章は75%の正確さで理解できるらしいですが、ぶっちゃけ75%の理解って理解したうちに入らないと思います。
90%でもなんかすごく嫌です。

10%わからないって相当わかってないと思うんですよね。

99%理解したいと考えると、単純計算して自分のlexile指数から400引いたぐらいがいいぐらいですかね。

lexile指数って、どうも線形で表現できているので、単純なモデルなんだと思います。もっといい指数が開発されてほしいですね。

個人的には↓の表のレベルの本

TOEICのリーディングスコア|ぼくがかんがえた読めるレベルのLexile指数|ネイティブのレベル|日本人のTOEIC受験者に関する情報
---|---|---
200|200L-295L|小1~2|中1・中3の受験者平均、大3・大4・大学院1の平均、英語専攻の大1・大2平均、海外経験半年未満の平均
250|200L-295Lや400L-495L|小1~4|中2・大学院2・大学院3の受験者平均、英語専攻の大3・大4平均、海外経験半年以上2年未満の平均、就職内定者の平均、TOEICの平均
300|400L-495L|小2~小4|大学院4の受験者平均、海外経験2年以上の平均、マスメディア勤務の平均(業界最高平均)、海外勤務の職種の平均
350|400L-495Lや600L-695L|小2~小6|TOEIC受験者のうちおよそ28.3%
400|600L-695L|小3~小6|TOEIC受験者のうちおよそ13.4%
450|600L-695Lや800L-895L|小4~中3|TOEIC受験者のうちおよそ3.6%
495|800L-895Lや1000L-1095L|小4~|不明
@|1200L-1295L|高2~|不明

だとスラスラ読めて楽しいレベルなんじゃないかなと思います。

TOEIC満点だと、だいたいネイティブの小4レベルだということっぽいです。

ちなみに、高校生のTOEICのリーディングスコア平均は200未満だったので省略しています。

(※参考 https://www.amazon.co.jp/%E8%8B%B1%E8%AA%9E-%E5%A4%9A%E8%AA%AD-lexile-%E6%B4%8B%E6%9B%B8/b?ie=UTF8&node=2480862051)
(※参考 http://www.iibc-global.org/library/default/toeic/official_data/lr/pdf/DAA.pdf)

それにしてもTOEIC Readingスコア0の人がこの600Lのやつを読めるとはおもえない(´・ω・｀)
```
Excuse me! Let's blow out of this place! In real life, germs are very small.
They can't be seen without a microscope.
Rudy forgot to use a tissue. His cold germs fly across the room at more than 100 miles an hour.
Whee! I can fly! Best ride ever! A few germs land on Ernie. But skin acts like a suit of armor.
It protects against harm. The germs won't find a new home there. Healthy skin keeps germs out.
But germs can sneak into the body through cuts, scrapes, or cracks in the skin.
Most germs enter through a person's mouth or nose. Rudy's germs continue to fall on nearly everything in the room - including Brenda's candy.
```

まあTOEICで点が取れたところでまだ「俺たちの戦いははじまったばかりだ！」的な感じなので、参考程度にということで(´・ω・｀)
