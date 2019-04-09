---
title: "シェーダーのバリエーション"
date: 2019-02-10T17:18:04+09:00
draft: false
categories: ["", ""]
description: ""
image: ""
tags: ["", ""]
author: ""
weight: 3
---

### arktoon/Opaque  
不透明なマテリアルの場合、こちらを設定してください。  
(オ(ｩ)ペークと読むらしいです）  
{{< figure src="/images/variant_opaque.jpg" >}}
### arktoon/AlphaCutout  
不透明と透明が明白に分かれている物体を表現する場合、こちらを指定してください。  
Main Textureの透明度でカットアウト（切り抜き）が行われます。  
影も切り抜いた形状で投写されます。  
{{< figure src="/images/variant_alphaCutout.jpg" >}}
### arktoon/Fade  
物体に半透明を含む場合、こちらを指定してください。  
落とす影も透明度に応じてディザリング処理されます。  
{{< figure src="/images/variant_fade.jpg" >}}
### arktoon/FadeRefracted  
物体に半透明を含み、かつ奥の映像を屈折させたい場合、こちらを指定してください。  
（パスが1個増えて多少負荷が増えるため、屈折が不要であればFadeを使ってください）  
{{< figure src="/images/variant_fadeRefracted.jpg" >}}
### arktoon/Stencil/Writer(またはReader)/Cutout
描画と同時に、ステンシルバッファの書き込み（Writer）、  
および読み込んで比較して表示制御（Reader）を実施します。  
それ以外の機能はCutoutと同等です。  
{{< figure src="/images/variant_stencil.jpg" >}}
### arktoon/Stencil/Reader/Fade
上記「arktoon/Stencil/Reader/Cutout」のFadeバリエーションになっています。
### arktoon/Stencil/WriterMask/Cutout
上記「arktoon/Stencil/Writer/Cutout」に、ステンシルバッファ専用のマスクテクスチャを追加したバリエーションになります。
{{< figure src="/images/variant_stencilWriterMask.jpg" >}}
### arktoon/Stencil/Reader/Double/FadeFade
ステンシル別で2回Fadeを描画します。それぞれPrimaryとSecondaryに分かれます。
「Main Texture」「Color」「Normal Map」「Emission」の４つはそれぞれ別で定義できます。
Primaryに「NotEqual」を指定し、SecondaryのColorを半透明にし「Equal」を指定することで、ステンシルの対象となった部分を半透明に透けさせることができます。
{{< figure src="/images/variant_stencilReaderFadeFade.jpg" >}}
### arktoon/_Extra/EmissiveFreak
下記機能が設定できる、アニメーション付きの発光テクスチャを2枚使用できる、特殊バリエーションです。  

- 色&テクスチャを指定可能
- マスクを指定可能（後述のスクロール・深度等のエフェクトの影響を受けない。）
- 色&テクスチャをスクロール
- 色&テクスチャに奥行きをつける(Parallaxed Emissionと同じ効果)
- いくつかの発光エフェクトと、それぞれの適用度を設定可能（ブリージング・ブリンク）
- カラーシフトアニメーションを設定可能(Hue Shift)

{{< figure src="/images/variant_EmissiveFreak.gif" >}}
  
