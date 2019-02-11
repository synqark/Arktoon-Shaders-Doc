---
title: "更新履歴"
date: 2019-02-11T11:33:07+09:00
draft: false
categories: ["", ""]
description: ""
image: ""
tags: ["", ""]
author: ""
weight: 6
---

***
## v1.0.1.1 (from v1.0.0)
#### アップグレードの時にやってほしいこと
- [Outline]→[Use Width Mask]にチェックを**入れてなかった**方  
このプロパティは廃止され、常時オンになったため、  
**アップグレード後[Outline]→[Width & Mask]にマスクテクスチャが指定されていれば、それを削除**してください。
- [Shadow]→[Use Custom Shade]をオンにして独自の陰を指定していた方  
**アップグレード後 [Shadow] カテゴリの [Strength & Mask] のスライダーを 1に**してください。

#### 変更点
- **レイアウトの修正を行いました。**  
細かいところで並び替え、文言修正などが行われています。    
![dyqspajuwaa_nqa](https://user-images.githubusercontent.com/10284218/52543830-20f77500-2df0-11e9-9cd4-ee4ef9a0c6fb.png)
- **ドキュメントのWebページ版を作成しました。**  
https://synqark.github.io/Arktoon-Shaders-Doc/  
Google Doc版は1.0.0.0を最終版とし、今後こちらをメンテナンスしていきます。
![image](https://user-images.githubusercontent.com/10284218/52543863-556b3100-2df0-11e9-91ea-722cc160f23d.png)
- **[Outline] カテゴリにカラーシフト機能を追加しました。**  
Color と Base Color Mixの計算後に、HSVシフトが行えます。  
![image](https://user-images.githubusercontent.com/10284218/52544768-45565000-2df6-11e9-86ba-6c559bc2057c.png)


- **[Use Custom Shade]がオンの場合でも、[Shadow]→[Strength & Mask]が使用できるようになりました。**  
**Custom Shadeの色を100%適用させたい場合、Strengthは常にMAXである必要があります**
- **[Outline]→[Use Width Mask]を廃止しました。**  
テクスチャが指定されていなければ、使わないと同義だったので。

***