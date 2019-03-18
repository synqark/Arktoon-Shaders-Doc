---
title: "Outline"
date: 2019-02-10T21:25:08+09:00
draft: false
categories: ["", ""]
description: ""
image: ""
tags: ["", ""]
author: ""
weight: 5
---

### できること
メッシュにアウトラインを設定できます。
{{< figure src="/images/cat_outline1.gif" >}}
### 各項目について
#### Width & Mask
アウトラインの幅を設定します。  
マスクとして白黒テクスチャを設定でき、スライダーの値に乗算され、場所ごとの幅の太さを設定できます。
#### Cutoff Mask / Cutoff Range
アウトラインを「描画しない」箇所をマスクテクスチャで指定します。  
Cutoff Rangeを操作して描画しない部分を調整できます。
#### Color & Texture
アウトラインの色をテクスチャ×カラーで設定できます。
#### Base Color Mix
CommonカテゴリのMain Colorの色を合成します。
#### Use Color Shift
ColorおよびBase Color Mixで決定された色に対して、HSVシフトを設定します。
#### Shadow mix
Shadowで設定した陰影をどの程度適用するかをスライダーで指定します。  
暗いところで光らせたくない場合にスライダーを1に設定してください。
