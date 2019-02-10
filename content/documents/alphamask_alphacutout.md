---
title: "AlphaMask / AlphaCutout"
date: 2019-02-10T21:16:21+09:00
draft: false
categories: ["", ""]
description: ""
image: ""
tags: ["", ""]
author: ""
weight: 2
---

## AlphaMask（Fade系列のバリエーション指定時に出現)
### できること
マテリアルの透明度を、グレースケールテクスチャで追加指定することがきます。  
{{< figure src="/images/cat_alphamask.jpg" >}}
### 各項目について
#### Alpha Mask
白黒テクスチャを指定すると、Commonカテゴリで指定した透明度を乗算します。  
Commonカテゴリでの透明度が1である場合、白黒テクスチャがそのまま透明度となります。  

## AlphaCutout (arktoon/AlphaCutout を指定時に出現）
### できること
カットアウトの閾値（Main Textureに設定された透明度がいくつまでは不透明、いくつまでは半透明かを判断する値）を設定できます。
{{< figure src="/images/cat_alphacutout.gif" >}}
### 各項目について
#### Cutoff Adjust
Main Textureのアルファの不透明/透明の閾値をスライダーで指定します。  
例：0.5が指定された場合、テクスチャのアルファ値が0～127が透明・128～255が不透明の扱いになります。  

