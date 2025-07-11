# ASCII Run Game

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

🎮 **ASCII風エフェクトで描画される3Dランニングゲーム**

three.jsのASCIIエフェクトを使用したユニークなビジュアルの無限ランナーゲームです。プレイヤーは敵を避けながら、踏んで倒しながら、できるだけ高いスコアを目指します。

## 🎯 ゲームの特徴

- **ASCII風3Dグラフィック**: three.jsのAsciiEffectによる独特なビジュアル
- **多層システム**: 地面、浮いているプラットフォーム、複数タイプの敵
- **コンボシステム**: 連続で敵を倒すとスコア倍率がアップ
- **動的難易度**: プレイヤーのスキルに応じて難易度が自動調整
- **豊富なエフェクト**: パーティクル、背景アニメーション、環境エフェクト
- **レスポンシブ対応**: デスクトップ・モバイル両対応

## 🎮 操作方法

- **ジャンプ**: `SPACE`キー / マウスクリック / タップ
- **二段ジャンプ**: 空中でもう一度ジャンプ可能
- **敵を踏む**: 敵の上から着地すると敵を倒せます
- **リスタート**: ゲームオーバー後、RESTARTボタンをクリック

## 🎯 ゲームシステム

### 敵の種類
- **地面の敵**: 地面を歩く基本的な敵（白色）
- **浮遊敵**: 上下に移動する敵（オレンジ色）
- **高高度浮遊敵**: 高い位置を移動する特別な敵（紫色）
- **プラットフォーム敵**: 浮いているプラットフォーム上を巡回する敵（ピンク色）

### スコアシステム
- 時間経過でスコア獲得
- 敵を倒すとボーナススコア
- コンボでスコア倍率アップ（最大5倍）

### 難易度システム
- 10秒ごとに難易度レベルが上昇
- 敵の移動速度とスポーン頻度が増加
- プレイヤースキルに応じた動的調整

## 🛠️ 技術仕様

- **フレームワーク**: Pure JavaScript (ES6 modules)
- **3Dライブラリ**: three.js v0.178.0
- **エフェクト**: AsciiEffect
- **レンダリング**: WebGL
- **CDN**: UNPKG (three.js)

## 🎨 ビジュアルエフェクト

- **4層背景システム**: 深宇宙、星座、雲、流れ星
- **環境エフェクト**: 草、花、石の配置
- **パーティクルシステム**: 爆発、ジャンプ、コンボエフェクト
- **動的アニメーション**: プレイヤー変形、背景の流れ

## 📁 ファイル構成

```
250708_ascii_run/
├── index.html          # メインゲームファイル
├── LICENSE             # MITライセンス（three.js含む）
└── README.md           # このファイル
```

## 🚀 実行方法

### ローカル開発
```bash
# HTTPサーバーが必要（ES6 modulesのため）
npm install -g http-server
cd 250708_ascii_run
http-server .
```

### GitHub Pages
1. GitHubリポジトリにプッシュ
2. Settings → Pages で `main` ブランチを選択
3. 生成されたURLでアクセス

## 📄 ライセンス

このプロジェクトはMITライセンスの下で公開されています。

### クレジット
- **Powered by three.js (MIT)** - © 2010-2025 three.js authors
- **Original ASCII Effect**: three.js "webgl_effects_ascii" example
- **Game Modification**: Keita Suezaki 2025

three.jsライブラリとそのサンプルコードの著作権は、three.jsの作者および貢献者に帰属します。

## 🔧 開発情報

### 依存関係
- three.js: v0.178.0 (CDN経由)
  - Core library: `three.module.js`
  - AsciiEffect: `effects/AsciiEffect.js`

### ブラウザ対応
- モダンブラウザ（ES6 modules対応）
- WebGL対応環境
- モバイルブラウザ対応

### パフォーマンス
- AsciiEffectは処理が重いため、低スペック端末では注意
- 必要に応じて解像度調整可能

## 🐛 既知の問題

- 一部のモバイル端末でパフォーマンスが低下する可能性
- 古いブラウザではES6 modulesが動作しない

## 🤝 コントリビューション

バグ報告や機能提案はIssueでお知らせください。プルリクエストも歓迎します。

---

**楽しいゲーム体験をお楽しみください！** 🎮✨ 