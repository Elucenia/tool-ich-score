<!-- ELUCENIA technical documentation · ich-score · zh · no clinical/professional/rights approval -->

# ICH Score

[条件、来源与许可](https://elucenia.org/zh/tools/ich-score)

## 使用方法

在门户中使用工具，或通过本地 HTTP 服务器打开 index.html。选择语言，填写各字段，然后计算。

## 输入与单位

### 格拉斯哥昏迷评分

`gcs`

- `0` — 13 至 15
- `1` — 5 至 12
- `2` — 3 至 4

### 血肿体积 ≥ 30 mL（ABC/2 公式）

`vol`

### 脑室内出血

`ivh`

### 幕下起源

`infra`

### 年龄 ≥ 80 岁

`idade`

## 方法版本

ICH/Hemphill 2001：5因素，总计0–6；体积ABC/2；无自动治疗决策

## 已记录的公式

Glasgow 3至4 = 2 · 5至12 = 1 · 13至15 = 0；体积≥ 30 mL = 1；脑室扩展=1；幕下起源=1；年龄≥ 80岁=1。总计0至6。

体积用ABC/2：A = 最大面积层面的血肿长径；B = 与A垂直的直径；C = 含血肿层面数×层厚（cm）。结果mL。

## 限制与适用人群

用于评估脑内出血初次就诊时的严重程度，在原始队列中与30天死亡率相关。年龄和出血体积是评分组成项。摘要没有证实单独评分可以支持治疗决定或确定个体的最终预后。

## 参考文献

- [Hemphill JC 3rd et al. The ICH score: a simple, reliable grading scale for intracerebral hemorrhage. Stroke, 2001.](https://doi.org/10.1161/01.STR.32.4.891)

## 复现技术测试

在此仓库的根目录中运行 node test.cjs，以重复已记录的合成案例。原始输入、预期结果和容差保持不变。技术测试不构成临床验证。

```sh
node test.cjs
```

tool.json 包含来源、版本和审查范围。examples.json 保留合成输入与预期结果；results.json 记录实际得到的结果。

[记录与参考文献](../tool.json) · [JavaScript代码](../calculator.js) · [参考案例](../examples.json) · [results.json](../results.json)

## 审查与使用条件

尚未开展独立临床审查。

此界面为自主编写的翻译，并非官方或认证版本。尚未完成独立临床审查、专业语言审查或工具权利授权。

公式或分类结果。解释、处理及适用性须结合专业评估和所选来源。

## 许可与署名

Apache-2.0 仅适用于 ELUCENIA 代码。工具、出版物、翻译和数据的权利仍归各自权利人所有。请保留 LICENSE 和 NOTICE。

ELUCENIA · Felipe Guedes · Copyright © 2026

## 已记录的结果

以下信息保留该方法对合成示例的输出，不构成独立的临床验证。

### 1

30 天死亡率：0%


### 2

30 天死亡率：26%


### 3

30 天死亡率：97%

