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
## v1.0.2.2 (from v1.0.1.1)
#### 変更点
- アウトラインカテゴリのカラーにテクスチャを指定できるようになりました
- UnityをProスキンで実行中に、一部テキストが非常に見づらくなる問題を修正しました
- 今後のバージョンアップ時の作業がやりやすくなりました。
今後は、導入済みのプロジェクトに新しいArktoon-Shadersをインポートした時点で、マテリアルのアップグレード処理が行われ、手動の変更作業がなくなる予定です。
    - （1.0.1.0以降のバージョンで作られたアバターに導入する方法）
無邪気にアバターと最新版のArktoon-Shaderをインポートして完了になります。

    - （0.9.5.3～1.0.0.0のバージョンのシェーダーで作られたアバターを導入する方へ）
①最初にそのアバターが想定しているArktoon-Shadersのバージョンをインポートしてください。
過去のバージョンはhttps://github.com/synqark/Arktoon-Shaders/releases からダウンロードできます
②その後、最新版のArktoon-Shadersをインポートしてください
今まで手動で作業が必要だった部分のアップグレードが自動で実施されます。

    - （0.9.5.3より前のバージョンのアバターに最新版のArktoon-Shadersを導入する方法）
最新版のArktoon-Shadersを導入後、https://github.com/synqark/Arktoon-Shaders/releases に記載されている0.9.5.3までの **インポート時の注意** の作業をお願いします（ごめんなさい）
- ビルド時間が早くなったかもしれません。
- Arktoonのアセットバージョンの更新を検知した際の**強制再インポート**処理は廃止しました。  
→これは、ビルド失敗（多重に見える、等）の暫定対応として実装していた機能でしたが、効果がみられなかったためです。
- ↑の代わりに、検知した時に存在する全てのArktoonマテリアルの設定変更を行うようになりました

#### 内部的な話
- テキストシリアライズ方式に変更しました
- シェーダーのコンパイルに関する大幅な仕様変更をしました。動きに影響はありません。
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