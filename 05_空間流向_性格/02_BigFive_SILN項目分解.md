# 02_BigFive_SILN項目分解

*RDL Human / T3 / DRAFT v1.1*  
*ファイル名は履歴上維持 / Core v2.3同期*

## 0. 目的

Big Five（OCEAN）を人間SILNの「内部部品」として同定するのでなく、**特定の測定Bで得られる反復的な応答傾向の圧縮断面**として再記述する。

```text
human SILN
↕ RIB群
↓ measurement B_trait
M_B / RIB_B
↓
responses / reports / behavior
↓ measurement Function
Big Five score
```

したがって `Big Five score ≠ Core variable` である。

## 1. Human側の対応候補

### Extraversion

外部相互作用への接近頻度・報酬期待・社会的刺激への応答等の組合せとして比較する。

### Agreeableness

協調・関係維持・対立回避・他者応答への感度等の観測断面として扱う。

### Conscientiousness

目標保持、計画継続、遅延報酬、規則・習慣の維持等の観測断面として扱う。

### Neuroticism

脅威感度、情動反応、回復時間、反復的な警戒等の観測断面として扱う。旧「誤差EをCore Hへ変換する係数」という定義は採用しない。

### Openness

新奇な経験・抽象的関係・再記述候補への接近傾向として扱う。旧「未確定領域ξへの重み」という定義は採用しない。新奇性は `ξ` ではない。

## 2. 数式の身分

SFOやHuman固有パラメータでBig Fiveを近似する式を置く場合、それは測定モデルの候補である。Core定義ではなく、データと耐久検査により採否を決める。

## 3. 注意

Big Fiveは観測尺度であり、人間の全構造を尽くさない。同じスコアでもB・文化・役割・状況が異なれば、相互作用応答は異なりうる。
