---
title: "Reflection"
date: 2019-02-10T21:27:30+09:00
draft: false
categories: ["", ""]
description: ""
image: ""
tags: ["", ""]
author: ""
weight: 7
---


### できること
メッシュに対して鏡面反射を設定します。
{{< figure src="/images/cat_reflection1.gif" >}}
### 各項目について
#### Use Reflection Probe
シーン中のReflection Probeを使用する場合はチェックします。
チェック無し、またはチェックがあってもシーンに存在しない場合はCubemapが使用されます。
#### Smoothness & Mask
面の「つやつや度」を設定します。高いほど光が集まり、強く反射します。
Maskを指定することでメッシュの部分部分で設定が可能です。
#### Cubemap（Fallback）
反射もととなるCubemapテクスチャを設定します。
Use Reflection Probeがオンの場合は、シーンに存在しない場合に自動的に設定されます。
#### Normal Map mix
Reflectionを着色する際にNormal mapをどの程度考慮するかをスライダーで指定します。
#### Shadow mix
陰影部分にどの程度Reflectionを適用”しない”かをスライダーで指定します。
#### Suppress Base Color
Reflectionの着色に応じてメッシュ本来の色（≒ Main Color）をどの程度「抑える」かをスライダーで設定します。
