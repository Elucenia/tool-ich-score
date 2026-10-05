<!-- ELUCENIA technical documentation · ich-score · ja · no clinical/professional/rights approval -->

# ICH Score

[条件・出典・許諾](https://elucenia.org/ja/tools/ich-score)

## 使い方

ポータルでツールを使用するか、ローカルHTTPサーバー経由でindex.htmlを開いてください。言語を選択し、項目を入力して計算してください。

## 入力項目と単位

### グラスゴー昏睡尺度

`gcs`

- `0` — 13 ～ 15
- `1` — 5 ～ 12
- `2` — 3 ～ 4

### 血腫体積 ≥ 30 mL（ABC/2式）

`vol`

### 脳室内出血

`ivh`

### テント下起源

`infra`

### 年齢 ≥ 80 歳

`idade`

## 方法の版

ICH/Hemphill 2001：5因子，合計0–6；血腫量ABC/2；自動治療判断なし

## 記載された計算式

Glasgow 3〜4 = 2 · 5〜12 = 1 · 13〜15 = 0；血腫量≥ 30 mL = 1；脳室穿破=1；テント下起源=1；年齢≥ 80歳=1。合計0〜6。

血腫量はABC/2：A = 最大面積スライスの血腫最大径；B = Aに垂直な径；C = 血腫スライス数×厚さ（cm）。結果mL。

## 限界・対象集団

脳内出血の初診時の重症度を推定し、原コホートでは30日死亡率と関連しました。年齢と血腫量はスコアの項目です。抄録は、スコアだけで治療判断や個人の確定的な予後を正当化できることを示していません。

## 参考文献

- [Hemphill JC 3rd et al. The ICH score: a simple, reliable grading scale for intracerebral hemorrhage. Stroke, 2001.](https://doi.org/10.1161/01.STR.32.4.891)

## 技術テストの再現

このリポジトリのルートディレクトリでnode test.cjsを実行すると、記録された合成ケースを再実行できます。元の入力、期待結果、許容誤差は保持されています。技術テストは臨床的検証を意味しません。

```sh
node test.cjs
```

tool.jsonには出典、版、確認範囲が記録されています。examples.jsonには合成入力と期待結果が保持され、results.jsonには実際に得られた結果が記録されています。

[記録・参考文献](../tool.json) · [JavaScriptコード](../calculator.js) · [参照ケース](../examples.json) · [results.json](../results.json)

## 確認状況と使用条件

独立した臨床レビューは実施されていません。

このインターフェースは独自に作成した翻訳であり、公式版や認証済みの版ではありません。独立した臨床レビュー、専門家による言語レビュー、評価尺度等の権利許諾の確認は実施されていません。

式または分類の結果です。解釈、対応、適用可能性は専門家による評価と選択した出典に依存します。

## ライセンスと帰属表示

Apache-2.0はELUCENIAのコードにのみ適用されます。評価尺度等、出版物、翻訳、データの権利は、それぞれの権利者に帰属します。LICENSEとNOTICEを保持してください。

ELUCENIA · Felipe Guedes · Copyright © 2026
