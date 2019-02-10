---
title: "Matcap"
date: 2019-02-10T21:26:05+09:00
draft: false
categories: ["", ""]
description: ""
image: ""
tags: ["", ""]
author: ""
weight: 6
---

### できること
メッシュに対して、予め「ライティングされた光源」（＝MaterialCapture, MatCap）テクスチャを設定できます。
{{< figure src="/images/cat_matcap1.gif" >}}
### 各項目について
#### (カテゴリバー）Blend Mode
MatCapの色をどのように合成するかを設定します。  
**Add:加算, Lighten:比較(明), Screen:スクリーン合成**  
となります
#### Blend & Mask
Blend Modeで設定した方法でどの程度ブレンドするかを設定します。  
マスクテクスチャを使うことで、メッシュの部分ごとのブレンドを制御できます
（黒色：0　～　白色：Blendの値）
#### Texture & Color
MatCapテクスチャと色を指定します。
#### Normal Map mix
MatCapを着色する際にNormal mapをどの程度考慮するかをスライダーで指定します。
#### Shadow mix
陰影部分にどの程度MatCapを適用”しない”かをスライダーで指定します。
