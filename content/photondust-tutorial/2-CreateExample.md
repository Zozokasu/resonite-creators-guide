---
title: 4.2. サンプルをいじってみる
---
## サンプルパーティクルの作成
テンプレートそして作成できるパーティクルシステムをいじりながらパーティクルを作ってみましょう。

[Dev Tool](../tool-usage/devTool.md)の`新規作成`から**Particle System**を選択してください。
>[!note]
> 画像予定

このようなサンプルのパーティクルが出現します。
![サンプルパーティクル](../image/newParticleSystem.webp)

このパーティクルにはつぶつぶを飛ばすためだけの最低限の機能がついています。

Slotの構造は以下のようになっています。
- ParticleSystem
  - Emitter
  - Material
  - Initializers
  - Simulators
### それぞれのSlotのなかみ
長いので飛ばしても大丈夫です。
#### ParticleSystem の中身
3つのコンポーネント、`ParticleSystem`、`ParticleStyle`、`BillboardParticleRenderer`がくっついています。

> [!abstract]- **ParticleSystem**（パーティクルシステム）
> パーティクルの基本設定をするコンポーネントです。設定できる内容は
> - どのParticleStyleを使うか
> - どの場所（Slot）を基準にするか
> - パーティクルは最大でどのくらいの数にするか
> - など
    > があります。

> [!abstract]- **ParticleStyle**（パーティクルスタイル）
> 1つのParticleRenderer（パーティクルレンダラー）と、複数のModule（モジュール）をもとにパーティクルの見た目や動きを決定します。
>
> 「いくつかのモジュールを組み合わせてParticle Styleをつくる」とも言い換えできます。

> [!abstract ]- **BillboardParticleRenderer**（ビルボードパーティクルレンダラー）
> パーティクルを2Dの画像として描画するようにするコンポーネントです。
#### Emitter Slotの中身
`Point Emitter`コンポーネントのみが入っています。
> [!abstract]- **Point Emitter**（ポイントエミッター）
> Slotがいる点からパーティクルを発生させるエミッターです。
> - どのくらいの頻度でパーティクルを出すか
> - どのParticleSystemを使うか
> - コンポーネントが有効化した（EnabledがTrueになった）ときにどのくらいのパーティクルをドバっと出すか（Burst）。その最小値と最大値。
> - パーティクルを放つ向き
#### Material Slotの中身

#### Initializers Slotの中身

#### Simulators Slotの中身

## 色を変えてみる
## 遠くまで飛ばしてみる
## 
## パーティクルをたくさん出してみる