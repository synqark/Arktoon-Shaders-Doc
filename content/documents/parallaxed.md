---
title: "Parallaxed Emission"
date: 2019-02-10T21:30:06+09:00
draft: false
categories: ["", ""]
description: ""
image: ""
tags: ["", ""]
author: ""
weight: 10
---

### できること
視差のあるEmissionテクスチャを貼り付けることができます。
### 各項目について
#### Texture / Color
表示させたいテクスチャを指定します。Colorを設定して乗算できます。
#### Mask
Parallaxed Emissionを適用する場所を、白黒のテクスチャで指定します。
#### Parallax Depth / Parallax Depth Mask
適用したいものの視差を設定します。
正の値だと手前にくるようになり、負の値だと奥に行ったようになります。
Parallax Depth Maskを指定することで、スライダーで指定したDepthの値に乗算します。
#### Invert Depth Mask
Depth Maskを逆にします。黒=1　～　白=0としてDepthの値を乗算します。
