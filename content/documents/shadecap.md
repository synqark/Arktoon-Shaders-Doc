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
### 各項目について
#### Blend Mode (Darken:比較(暗), Multiply:乗算, Light Shutter:受光マスキング）
ShadeCapをどのように合成するかを決定します
#### Blend / Blend Mask
Blend Modeで設定した方法でどの程度ブレンドするかを設定します。マスクテクスチャを使うことで、メッシュの部分ごとのブレンドを制御できます
（黒色：0　～　白色：Blendの値）
#### Normal Map mix
ShadeCapを着色する際にNormal mapをどの程度考慮するかをスライダーで指定します。
#### Texture / Color
MatCapテクスチャと色を指定します。
今のところColorは意味を成しません。
