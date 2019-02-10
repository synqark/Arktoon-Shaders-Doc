---
title: "Advanced"
date: 2019-02-10T21:30:57+09:00
draft: false
categories: ["", ""]
description: ""
image: ""
tags: ["", ""]
author: ""
weight: 11
---

### なにこれ？
説明が面倒だったり普段使わなかったり、実験的な設定項目をここに隠しています。
{{< figure src="/images/cat_advanced.jpg" >}}
### 各項目について
#### Lights → Sampling Style (デフォルト：Arktoon）
間接光の取得条件を オリジナル(Arktoon)　および Cubed-Unity-Shader (Cubed)の2択から選択できます。
#### Directional Shadow → Indirect face Intensity（デフォルト：0.25）
「陰色」の明るさを微調整します  
Shadow Strengthと似たような感じですが、「陰色」の強度ではなく、「陰色」そのものを決定します。  
Vertex Colors → Color blend to [diffuse, emissive] (デフォルト：0）  
メッシュに頂点カラーがある場合、こちらのスライダーを上げることで、  
Diffuse (≒Main Texture） / Emissive にその色を乗せることができます。
#### PointLights
「平行光源ではないリアルタイムライト」から受ける光の陰影の強さ・境界などを設定します。　  
PointLight Shadows → Use Per-vertex Light（デフォルト：オン）  
「頂点ライティング」モードのポイントライトから光を受けるかを設定します。  
基本的にオンで良いですが、Cubed-Shaderなど他のシェーダーと光の当たり方を合わせる時や、鏡の奥で輪郭の点滅が気になる場合はオフにしてください。
#### Shade from other meshes
「他のメッシュから受けた影」とみなすための計算材料です。
基本的に無視してください。
#### MatCap / ShadeCap
MatCapやShadeCapで使用している計算式を切り替えます。
