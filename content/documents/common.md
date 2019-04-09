---
title: "Common"
date: 2019-02-10T21:10:57+09:00
draft: false
categories: ["", ""]
description: ""
image: ""
tags: ["", ""]
author: ""
weight: 1
---

### できること
そのマテリアルの基本となる色の設定ができます。
{{< figure src="/images/cat_common1.gif" >}}
### 各項目について
#### Main Texture
マテリアルの基本色をテクスチャ×カラーで指定します。  
ここで設定された色は影や周囲の色の影響を受けます。  
#### Normal Map
マテリアルの凹凸を表現するテクスチャを指定します。  
また指定されたテクスチャの強度をスライダーで設定できます。  
#### Emission
マテリアルが発光している色をテクスチャ×カラーで設定します。  
ここで指定された色は影や周囲の色の影響を受けません。
#### Is Double Sided
裏面を描画するかどうかを設定します。
（Cull Offではなく、裏面分の面を追加で生成しています）
##### Flip backface normal
裏面の法線を反転します。  
両面に設定したいメッシュが鉄などといった光を通さないものの場合に、適切な受光を設定します。　
##### Backface Light intensity
裏面の受光量を乗算で指定します。  
スカートの裏側など、必然的に暗い部分に関して倍率を下げることで自然な表現ができます。
{{< figure src="/images/cat_common2.gif" >}}
##### Use backface color shift
裏面の色をベースカラーから変更したいときに指定します。
{{< figure src="/images/cat_common3.gif" >}}
#### ZWrite （arktoon/Fade を指定時に表示）
透明に関する設定です。基本的にはONで触る必要がありませんが、  
負荷を考慮したい場合や、ONが意図した透過表現でない場合に変更してみてください。