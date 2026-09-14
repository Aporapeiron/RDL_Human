# RDL Human

**RDL_Human** は、RDL Core を人間・身体・認知・情動・行動・社会へ適用する **T3 応用層**である。

*同期基準：RDL_Core BASE / SPEC v2.3、RDL_Functions 現行版、RDL_Durability_Modules 現行版*

## 0. 位置づけ

```text
RDL_Core
  T0: SILN / B / M_B / RIB / RIB_B / ξ
  T1: 展開 → 検査・選別 → 再構成
        ↓
RDL_Functions
  有限B・入出力契約を持つ演算モジュール
        ↓
RDL_Durability_Modules
  維持域・変形域・遷移域・破断域を検査
        ↓
RDL_Human
  人間・身体・認知・社会へ応用
```

Human は Core を再定義しない。人間固有の「熱」「流れ」「自己境界」「認知空間」「SFO」「実効拘束場」等は、**T3 の仮説変数・比喩・操作モデル**であり、Core 記号と自動的に同一視しない。

## 1. Human適用の基本規律

```text
人間 / 人格 ≠ M_B
未知刺激 / 新奇性 / ノイズ ≠ ξ
Human側の心理的「熱」 ≠ Core H
Human側の「自己境界」仮説 ≠ Core Bそのもの
SILN は B によって生成されない
RIB_B ≠ F
Function ≠ M_B
```

```text
対象SILN / SILN群
      ↕ {RIB_i}
Purpose / B
      ↓
M_B + RIB_B
      ↓
F = interp(M_B, RIB_B)
      ↓
必要な場合のみ E / H / θ
      ↓
維持 / M_Δ / 再構成
```

`M_B` は「人間そのもの」「人格そのもの」ではなく、Bのもとで保持した有限な構造断面である。`ξ` は未知刺激・新奇性・欠測・ノイズ・心理的エネルギーではなく、有限Bで未回収関係が残るという Core 条件である。

## 2. Human固有仮説の扱い

4層時間スケール、認知空間、実効拘束場、SFO、流体比喩、放熱比喩等は、

```text
Human-specific model
= Core上で試す有限な説明モデル
≠ Core Primitive
≠ 医学・心理学上の確定事実
≠ 人間の本質的分類
```

として扱う。神経伝達物質・心理特性・社会理論との対応は、因果同定ではなく操作的対応候補として保持する。

## 3. 耐久検査

```text
Human hypothesis
↓
baseline M_B / RIB_B / F
↓
shake / remove / B-change / history / constraint / simulation
↓
維持 / 変形 / 遷移 / 破断
↓
残存関係と適用範囲を記録
```

壊れなかった仮説を真理へ昇格させず、「検査範囲内でまだ使える」と記録する。

## 4. 現在の構成

- `01_基層構造_神経力学/` — 時間スケール・反応特性・状態遷移の現行Human仮説
- `02_関係ネットワーク行動力学/` — 身体・道具・他者・制度との相互作用とFlow
- `03_認知_情動_放熱/` — 快・笑い・洞察・葛藤・主観時間の現行モデル＋旧研究ノート
- `04_身体_移動_流れ/` — 身体・移動・思考・感情のFlow比較
- `05_空間流向_性格/` — SFO・Big Five・MBTIの現行翻訳＋旧研究ノート
- `06_対話_倫理_社会生態系/` — 対話・倫理の現行文書＋地域・教育の旧研究ノート
- `07_既知学問のRDL翻訳ツリー/` — role mapping方式の現行翻訳
- `01_Language/` — 言語・共有文脈・言語変化
- `SSDからの翻訳/` — **RDL v2.0 時点の翻訳アーカイブ。pre-v2.3。現行定義の根拠には使わない**
- `_archive/` — 元原稿・歴史資料。現行定義の根拠には使わない

各フォルダーではREADMEの `CURRENT` / `PRE-v2.3 REFERENCE` 区分を優先する。

## 一文圧縮

> **RDL_Human は、人間を固定属性の集合として断定するのではなく、SILNとRIB群の相互作用を有限なBで記述し、Human固有仮説を耐久検査しながら使うT3応用層である。**
