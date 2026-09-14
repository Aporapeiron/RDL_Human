# 02_動ける個体のSILN分解と流体移動

*RDL Human / T3 / DRAFT v1.1*  
*Core v2.3同期*

## 0. 一文定義

> **空間を能動的に移動する個体をSILNとして対象化し、感知・経路選択・駆動・慣性等の機能を有限に分解して、環境との相互作用RIB群の中で位置更新がどう成立するかを記述するHuman側モデル。**

`SILN分解` はBによってSILNを生成したり、SILNを存在論的な部品へ切断する意味ではない。

## 1. Core接続

```text
mobile SILN
↕ environment / body / tool RIB群
↓ Purpose / B_move
RIB_B^move
+
M_B^move
↓
F_move
↓
Human側 navigation / action model
```

## 2. 機能分解

有限モデル上、次の機能を区別できる。

1. **Sensor** — 障害物・他者・地形・身体状態等の取得経路
2. **Navigator** — 目標・障害・コストから経路候補を形成
3. **Actuator** — 筋力・車輪・推進等の行為出力
4. **Inertia / dynamics** — 速度・質量・応答遅延等の物理制約

Sensorが受けるものを旧 `EFP` と呼ばず、環境との相互作用からBで取得した `RIB_B^move` とする。

## 3. 流体移動比喩

環境中の移動を「流体的」と呼ぶのは、障害物・他者流・目標勾配を滑らかに回避・追従する経路モデルを作るための比喩である。

$$
\frac{d\vec{v}}{dt} = -\frac{1}{\rho}\nabla V(x) + \nu \nabla^2 \vec{v} + \vec{F}_{goal}
$$

この式はHuman側の運動モデル候補であり、心理・社会現象がNavier–Stokes方程式そのものに従うという主張ではない。

## 4. フィードバック

```text
RIB_B(t) → F_move(t) → action
                         ↓
                  environment changes
                         ↓
                 RIB_B(t+Δ)
```

移動は「入力→出力」の一方向ではなく、行動によって次の相互作用条件が変わる閉ループとして扱う。
