---
title: "Rim"
date: 2019-02-10T21:28:17+09:00
draft: false
categories: ["", ""]
description: ""
image: ""
tags: ["", ""]
author: ""
weight: 8
---

### できること
メッシュのリム（ヘリ、枠）に対する光を指定できます（リムライトと呼ばれます）
### 各項目について
#### Blend / Blend Mask
Rimをどの程度着色するかを設定します。マスクテクスチャを使うことで、メッシュの部分ごとのブレンドを制御できます
（黒色：0　～　白色：Blendの値）
#### Shadow mix
陰影部分にどの程度Rimを適用”しない”かをスライダーで指定します。
#### Fresnel Power
フレネル強度を設定します。高いほど外側に着色が寄っていきます
#### Upper side width
リムライトの縁の太さを設定します。この値とFresnelPowerの値を上げることで
メッシュ内部でアウトラインを表現するのに使用できます。
#### Use Base Color
Main Textureで設定している色を使います。
#### Color / Texture
リムの色をカラーおよびテクスチャで設定します。
[Use Base Color]が設定されている場合、Main Textureの色と乗算します。