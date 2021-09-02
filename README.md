<img width="" alt="無題" src="https://user-images.githubusercontent.com/58076642/131785398-90ff623b-3ea2-492c-a148-87d20cbfa3cd.png">

# Kaggle Optiver Realized Volatility Prediction

## コンペの目的
株のボラティリティ(価格変動の度合い)を時間(time id)ごとに予測する。

## 評価指標
平均二乗パーセント誤差の平方根（RMSPE：Root Mean Squared Percentage Error）    

![CodeCogsEqn](https://user-images.githubusercontent.com/58076642/131785016-cb37749d-bf18-48e8-bd00-e06c60df471d.png)



### Overview(deepl)
ボラティリティは、トレーディングフロアで最もよく耳にする言葉の一つですが、それには理由があります。金融市場では、ボラティリティーは価格の変動量を表します。ボラティリティが高いということは、市場が乱高下し、価格が大きく変動していることを意味し、一方、ボラティリティが低いということは、より穏やかで落ち着いた市場を意味します。オプティバーのような取引会社にとって、ボラティリティを正確に予測することは、価格が原商品のボラティリティに直接関係するオプションの取引に不可欠です。

オプティバーは、世界有数の電子マーケットメーカーとして、金融市場の継続的な改善に取り組んでおり、世界中の数多くの取引所で、オプション、ETF、現物株式、債券、外国通貨へのアクセスと価格の向上を実現しています。オプティバーのチームは、数え切れないほどの時間をかけて、ボラティリティーを予測し、最終投資家にとってより公平なオプション価格を継続的に生成する高度なモデルを構築してきました。しかし、業界をリードする価格決定アルゴリズムは進化を止めることはできません。オプティバーがそのモデルを次のレベルに引き上げるために、Kaggleほど最適な場所はありません。

このコンペティションでは、最初の3ヶ月間で、様々なセクターの数百銘柄の短期的なボラティリティを予測するモデルを構築していただきます。何億行もの非常に詳細な財務データを手に入れ、それをもとに10分間のボラティリティーを予測するモデルを設計します。作成したモデルは、トレーニング後の3ヶ月間の評価期間に収集した実際の市場データと比較して評価されます。

このコンペティションを通じて、皆さんはボラティリティーと金融市場の構造に関する貴重な洞察を得ることができます。また、オプティバーが何十年にもわたって直面してきたデータサイエンスの問題についても、より深く理解することができるでしょう。私たちは、Kaggleコミュニティがこの複雑でエキサイティングなトレーディング課題にクリエイティブなアプローチを適用することを楽しみにしています。

### Data(deepl)
このデータセットには、金融市場での実際の取引の実行に関連する株式市場データが含まれています。特に、オーダーブックのスナップショットと約定した取引が含まれています。1秒の分解能で、現代の金融市場のミクロ構造を独特のきめ細かさで見ることができます。

### awards.csv colomn infomaiton

| name | Explanation |
| --- | --- |
| awardDate  | 賞を受賞した日 |
| awardSeason  | 賞を受賞したシーズン |
| awardId | ID |
| awardName | 賞の名前 |
| playerId | プレイヤーに一意に与えられているID |
| playerName | プレイヤーの名前 |
| awardPlayerTeamId | 受賞した選手が所属するチームID |

### example_sample_submission.csv colomn infomaiton

| name | Explanation |
| --- | --- |
| date  | 日付 |
| date_playerId  | 日付とplayerIDを連結したもの。目的変数を予測するためのkeyになっている |
| target1 | 目的変数1 |
| target2 | 目的変数2 |
| target3 | 目的変数3 |
| target4 | 目的変数4 |

