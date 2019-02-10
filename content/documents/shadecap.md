---
title: "Shadecap"
date: 2019-02-10T21:29:02+09:00
draft: false
categories: ["", ""]
description: ""
image: ""
tags: ["", ""]
author: ""
weight: 9
---

### できること
メッシュに対して、予め「ライティングされた陰」テクスチャを設定できます。  
MatCapの暗い版です。造語です。
{{< figure src="/images/cat_shadecap.gif" >}}
### 各項目について
#### (カテゴリバー）Blend Mode
MatCapの色をどのように合成するかを設定します。  
**Darken:比較(暗), Multiply:乗算, Light Shutter:受光マスキング**  
となります
##### Light Shutter:受光マスキングについて
これは合成方法ではなく、Shade Cap テクスチャを光を受けている箇所にマスキングします。  
つまり、黒いテクスチャを指定するとメッシュ全体が陰に入ったようになり、  
白いテクスチャを指定すると何も起きてないように見えます。
#### Blend & Mask
Blend Modeで設定した方法でどの程度ブレンドするかを設定します。マスクテクスチャを使うことで、メッシュの部分ごとのブレンドを制御できます
（黒色：0　～　白色：Blendの値）
#### Texture
ShadeCapテクスチャを指定します。
#### Normal Map mix
ShadeCapを着色する際にNormal mapをどの程度考慮するかをスライダーで指定します。
