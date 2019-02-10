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
### 各項目について
#### Blend Mode (Add:加算, Lighten:比較(明), Screen:スクリーン合成）
MatCapの色をどのように合成するかを設定します。
#### Blend / Blend Mask
Blend Modeで設定した方法でどの程度ブレンドするかを設定します。マスクテクスチャを使うことで、メッシュの部分ごとのブレンドを制御できます
（黒色：0　～　白色：Blendの値）
#### Normal Map mix
MatCapを着色する際にNormal mapをどの程度考慮するかをスライダーで指定します。
#### Shadow mix
陰影部分にどの程度MatCapを適用”しない”かをスライダーで指定します。
#### Texture / Color
MatCapテクスチャと色を指定します。
