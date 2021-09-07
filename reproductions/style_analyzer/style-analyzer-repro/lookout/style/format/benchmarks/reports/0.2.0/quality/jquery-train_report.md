# Train report for javascript / file:///tmp/top-repos-quality-repos-4md0ht25/jquery HEAD dae5f3ce3d2df27873d01f0d9682f6a91ad66b87

### Classification report

PPCR: 0.898

| Class | Precision | Recall | Full Recall | F1-score | Full F1-score | Support | Full Support | PPCR |
|------:|:----------|:-------|:------------|:---------|:---------|:--------|:-------------|:-----|
| `∅` | 0.988| 0.995| 0.989| 0.991| 0.988| 87319| 87836| 0.994 |
| `␣` | 0.962| 0.990| 0.938| 0.976| 0.950| 72911| 76959| 0.947 |
| `"` | 1.000| 1.000| 1.000| 1.000| 1.000| 32763| 32775| 1.000 |
| `⏎` | 0.973| 0.707| 0.208| 0.819| 0.343| 2852| 9677| 0.295 |
| `⏎⇥⁻` | 0.919| 0.814| 0.493| 0.863| 0.642| 2834| 4677| 0.606 |
| `⏎⇥⁺` | 0.000| 0.000| 0.000| 0.000| 0.000| 830| 5049| 0.164 |
| `⏎⏎` | 0.000| 0.000| 0.000| 0.000| 0.000| 504| 4975| 0.101 |
| `⏎⏎⇥⁺` | 0.921| 0.859| 0.468| 0.889| 0.620| 270| 496| 0.544 |
| `␣␣` | 0.000| 0.000| 0.000| 0.000| 0.000| 174| 197| 0.883 |
| `⏎⏎⇥⁻` | 0.000| 0.000| 0.000| 0.000| 0.000| 50| 619| 0.081 |
| `⏎⇥⁻⇥⁻` | 0.000| 0.000| 0.000| 0.000| 0.000| 41| 124| 0.331 |
| `micro avg` | 0.979| 0.979| 0.879| 0.979| 0.926| 200548| 223384| 0.898 |
| `macro avg` | 0.524| 0.488| 0.372| 0.503| 0.413| 200548| 223384| 0.898 |
| `weighted avg` | 0.971| 0.979| 0.879| 0.975| 0.892| 200548| 223384| 0.898 |

### Confusion matrix

|refusal|  ∅| ␣| "| ⏎| ⏎⇥⁺| ⏎⇥⁻| ⏎⏎| ⏎⏎⇥⁻| ⏎⏎⇥⁺| ␣␣| ⏎⇥⁻⇥⁻| 
|:---|:---|:---|:---|:---|:---|:---|:---|:---|:---|:---|:---|
|0 |0 |0 |0 |0 |0 |0 |0 |0 |0 |0 |0 |
|517 |86841 |468 |0 |0 |0 |10 |0 |0 |0 |0 |0 |
|4048 |690 |72181 |0 |0 |0 |39 |0 |0 |1 |0 |0 |
|12 |0 |0 |32763 |0 |0 |0 |0 |0 |0 |0 |0 |
|6825 |226 |568 |0 |2017 |0 |41 |0 |0 |0 |0 |0 |
|4219 |120 |701 |0 |4 |0 |0 |0 |0 |5 |0 |0 |
|1843 |16 |496 |0 |16 |0 |2306 |0 |0 |0 |0 |0 |
|4471 |1 |421 |0 |23 |0 |46 |0 |0 |13 |0 |0 |
|569 |0 |13 |0 |0 |0 |36 |0 |0 |1 |0 |0 |
|226 |0 |25 |0 |13 |0 |0 |0 |0 |232 |0 |0 |
|23 |0 |174 |0 |0 |0 |0 |0 |0 |0 |0 |0 |
|83 |4 |7 |0 |0 |0 |30 |0 |0 |0 |0 |0 |

### Files with most errors

| filename | number of errors|
|:----:|:-----|
| test/unit/event.js | 356 |
| test/unit/core.js | 274 |
| test/unit/offset.js | 250 |
| test/unit/ajax.js | 241 |
| test/unit/css.js | 202 |
| test/unit/wrap.js | 197 |
| test/unit/manipulation.js | 144 |
| test/unit/traversing.js | 139 |
| src/ajax.js | 138 |
| test/unit/attributes.js | 126 |

<details>
    <summary>Machine-readable report</summary>
```json
{
  "cl_report": {"\"": {"f1-score": 1.0, "precision": 1.0, "recall": 1.0, "support": 32763}, "macro avg": {"f1-score": 0.5034737568851518, "precision": 0.5238885689754146, "recall": 0.48769879721650505, "support": 200548}, "micro avg": {"f1-score": 0.9790174920717235, "precision": 0.9790174920717235, "recall": 0.9790174920717235, "support": 200548}, "weighted avg": {"f1-score": 0.974706241247474, "precision": 0.9712451160119105, "recall": 0.9790174920717235, "support": 200548}, "\u2205": {"f1-score": 0.9912394345297545, "precision": 0.9879746979453458, "recall": 0.9945258191229859, "support": 87319}, "\u23ce": {"f1-score": 0.8190862944162438, "precision": 0.9729860106126387, "recall": 0.7072230014025246, "support": 2852}, "\u23ce\u21e5\u207a": {"f1-score": 0.0, "precision": 0.0, "recall": 0.0, "support": 830}, "\u23ce\u21e5\u207b": {"f1-score": 0.8633470610258331, "precision": 0.919457735247209, "recall": 0.8136908962597036, "support": 2834}, "\u23ce\u21e5\u207b\u21e5\u207b": {"f1-score": 0.0, "precision": 0.0, "recall": 0.0, "support": 41}, "\u23ce\u23ce": {"f1-score": 0.0, "precision": 0.0, "recall": 0.0, "support": 504}, "\u23ce\u23ce\u21e5\u207a": {"f1-score": 0.8888888888888888, "precision": 0.9206349206349206, "recall": 0.8592592592592593, "support": 270}, "\u23ce\u23ce\u21e5\u207b": {"f1-score": 0.0, "precision": 0.0, "recall": 0.0, "support": 50}, "\u2423": {"f1-score": 0.9756496468759503, "precision": 0.961720894289445, "recall": 0.9899877933370822, "support": 72911}, "\u2423\u2423": {"f1-score": 0.0, "precision": 0.0, "recall": 0.0, "support": 174}},
  "cl_report_full": {"\"": {"f1-score": 0.9998169001190149, "precision": 1.0, "recall": 0.9996338672768879, "support": 32775}, "macro avg": {"f1-score": 0.4130310705982232, "precision": 0.5238885689754146, "recall": 0.37231330306105265, "support": 223384}, "micro avg": {"f1-score": 0.9262806299123444, "precision": 0.9790174920717235, "recall": 0.8789349281953944, "support": 223384}, "weighted avg": {"f1-score": 0.892172365598774, "precision": 0.9299696855881953, "recall": 0.8789349281953944, "support": 223384}, "\u2205": {"f1-score": 0.9883232612926355, "precision": 0.9879746979453458, "recall": 0.9886720706771711, "support": 87836}, "\u23ce": {"f1-score": 0.3433191489361702, "precision": 0.9729860106126387, "recall": 0.20843236540250076, "support": 9677}, "\u23ce\u21e5\u207a": {"f1-score": 0.0, "precision": 0.0, "recall": 0.0, "support": 5049}, "\u23ce\u21e5\u207b": {"f1-score": 0.6418928322894919, "precision": 0.919457735247209, "recall": 0.49305110113320505, "support": 4677}, "\u23ce\u21e5\u207b\u21e5\u207b": {"f1-score": 0.0, "precision": 0.0, "recall": 0.0, "support": 124}, "\u23ce\u23ce": {"f1-score": 0.0, "precision": 0.0, "recall": 0.0, "support": 4975}, "\u23ce\u23ce\u21e5\u207a": {"f1-score": 0.6203208556149732, "precision": 0.9206349206349206, "recall": 0.46774193548387094, "support": 496}, "\u23ce\u23ce\u21e5\u207b": {"f1-score": 0.0, "precision": 0.0, "recall": 0.0, "support": 619}, "\u2423": {"f1-score": 0.9496687783281693, "precision": 0.961720894289445, "recall": 0.9379149936979431, "support": 76959}, "\u2423\u2423": {"f1-score": 0.0, "precision": 0.0, "recall": 0.0, "support": 197}},
  "ppcr": 0.8977724456541203
}
```
</details>