---
title: フェイストラッキング
tags:
  - チュートリアル
date: 2025-04-27
---

## フェイストラッキングをする
### Vive Pro Eye・Vive Facial Tracker
- デフォルトで対応しています。基本的に特別な設定は必要ありません。

### VR（SteamLink）
SteamLinkがResoniteに表情データを送ってくれるように設定する必要があります。

1. SteamVR内で設定を開いて、左下のボタンで詳細設定を『表示』に切り替える
2. 以下の3つの設定をオンに切り替える
    - OSCを有効化
    - OSC経由でこのPCの他のアプリにアイトラッキングデータを共有
    - OSC経由でこのPCの他のアプリにフェイストラッキングデータを共有
3. 『OSC出力ポート』を『9000 (DIRECT)』に設定

- ほとんどの場合、この時点で目が動くようになります。口が動かない場合、アバター側の設定が必要です（以下を参照）。

#### 参考になる記事
- [(Quest Proでフェイストラッキングしよう orange著)](https://note.com/orange3134/n/n1b5ea13e5d5b)
    - いくつかのトラブルシューティングも載っています。
### VR（VirtualDesktop）
- Modを導入する必要があります（今のところ）。
    - https://github.com/Zeitheron/VDFaceTracking
        - [前提mod（ResoniteModLoader）](https://github.com/resonite-modding-group/ResoniteModLoader)が必要です

ここを読んでる人は結構な玄人だと思うので詳しい説明は省きます。

### デスクトップモードでのフェイストラッキング
https://github.com/Ruzeh3D/NeosWCFaceTrack/wiki/Installation

フェイストラッキング情報をWebSocket経由でResoniteに送信するソフトと、Resonite側の受信用アイテムのセットです。

NeosVR用のツールとなっていますがResoniteでも動くはずです。適宜Resoniteのものに読み替えてセットアップしてください。