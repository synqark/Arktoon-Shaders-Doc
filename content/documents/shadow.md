---
title: "Shadow"
date: 2019-02-10T21:19:37+09:00
draft: false
categories: ["", ""]
description: ""
image: ""
tags: ["", ""]
author: ""
weight: 3
---

### できること
マテリアルの陰に関する調整ができます。  
陰の強さだけではなく、陰の諧調、また陰にかかったテクスチャの色などを指定できます。  
{{< figure src="/images/cat_shadow1.gif" >}}
### 各項目について
#### Border
影の境目となる地点を指定できます。
#### Strength / Strength Mask
　陰影の暗さをスライダーで指定します。  
　また、必要に応じてマスクテクスチャを使いStrengthの値を乗算できます。  
　（ドローツールにある一般的なマスクと同じ意味です。）  
　「顔を除いて全体に陰を付けたい」などの場合は、顔だけを黒く、それ以外を白く塗りつぶしたテクスチャを設定して実現できます。  
　※Custom Shadeを使用中は設定ができません。  
#### Blur / Blur Mask
影の境目をどの程度グラデーションさせるかを指定します。0で境目がくっきりします。  
Border blur Maskを使うことで、下記の画像のように同一メッシュ内でも陰影の間隔を設定できます。
{{< figure src="/images/cat_shadow5.png" >}}
#### Use Steps / Steps
　Shadow borderで指定した陰のグラデーションをポスタライズ（n諧調化）する場合にチェックします。  
スライダーで指定した数字（小数点は切り捨て）分に色が切り分けられます。
#### Use Custom Shade
陰の部分をシェーダーに任せずに、独自で色またはテクスチャを指定したい場合にチェックします。
{{< figure src="/images/cat_shadow2.gif" >}}
#### Mix Default Shade
下記で設定した色に対して、シェーダーが決めた「本来の陰の色」の合成割合を指定します
#### 1st shade
以降のオプションは、1つ目の陰に対して適用されます。
#### Use Shade Texture → Shade Texture
陰にあたる部分をテクスチャを使って表現したい場合、設定します。  
（より良いサンプル動画募集してます..）
{{< figure src="/images/cat_shadow3.jpg" >}}
#### Hue Shift / Saturation / Value
陰にあたる部分を「色相/彩度/明度」を変更して設定する場合は、Shade Textureにチェックを入れずにスライダーで設定します。
{{< figure src="/images/cat_shadow4.jpg" >}}
#### 2nd shade (実験中の機能）
チェックすると、1つ目の陰と同様のオプションが表示されます。
