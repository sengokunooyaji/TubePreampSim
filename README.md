# Tube Preamp Simulator

ブラウザ上で動く真空管プリアンプの回路シミュレーターです。

🌐 **Live Demo:** [https://sengokunooyaji.github.io/TubePreampSim/](https://sengokunooyaji.github.io/TubePreampSim/)

## 概要 (Overview)
回路図の定数から、各段の動作点・周波数特性・波形と歪みを計算します。
真空管はKorenモデルを使用し、節点解析（直流・交流・過渡解析）をフロントエンドのJavaScriptのみで完結して実行しています。

## 主な機能 (Features)
* **周波数特性の解析:** RIAA補正やトーンコントロール（バクサンドール型）を含む総合特性のグラフ表示。
* **波形・歪みの計算:** 1kHzの過渡解析から求めた入出力カーブによる高調波スペクトル（THD）の算出。
* **Web Audio APIによる試聴:** 手元の音声ファイル（WAV, MP3, FLAC等）を画面にドラッグ＆ドロップし、シミュレートされたアンプ特性を通してリアルタイムに比較試聴。
* **直流動作点の確認:** プレート電圧、カソード電圧、グリッド電流や損失超過などのステータス警告表示。

## 使い方 (Usage)
サーバー側の処理やインストールは一切不要です。Live Demoのリンクにアクセスするか、リポジトリ内の `index.html` をダウンロードしてブラウザで開くだけで動作します。

## 技術仕様 (Tech Stack)
* HTML5 / CSS3 / Vanilla JavaScript
* Canvas API (グラフ描画)
* Web Audio API (音声処理・リアルタイム波形整形)
* 外部ライブラリ非依存 (No external dependencies)

## ライセンス (License)
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
