# OpenPose(tf-pose-estimation)_Windows_environment-setup
WindowsにOpenPoseを環境構築する方法

## 1) OpenPose 1.7.0 のインストール
下記URLの「Assets」から各PCに応じたzipファイルをダウンロードする。
https://github.com/CMU-Perceptual-Computing-Lab/openpose/releases

<CPU版をダウンロードする場合>

openpose-1.7.0-binaries-win64-cpu-python3.7-flir-3d

<GPU版をダウンロードする場合>
*GPU: コンピュータゲームに代表されるリアルタイム画像処理に特化した演算装置あるいはプロセッサ

openpose-1.7.0-binaries-win64-gpu-python3.7-flir-3d_recommended

※以下，CPU版をダウンロードした場合の流れで記載

## 2) ダウンロードしたzipファイルの展開（解凍）
C:\ の直下に 展開（解凍）するなど，分かりやすいディレクトリに置く。

C:\ の直下に展開（解凍）した場合，openpose-1.7.0-binaries-win64-cpu-python3.7-flir-3d のようなディレクトリができることを確認。

## 3) Pathの追加
Windows での環境変数の設定は，マイコンピュータを右クリック → プロパティ→ 詳細設定 → 環境変数をクリック

* システム環境変数: Path

* 追加する値: C:\openpose-1.7.0-binaries-win64-cpu-python3.7-flir-3d\openpose\bin

## 4) modelsの下の getBaseModels.bat を実行
cd C:\openpose-1.7.0-binaries-win64-cpu-python3.7-flir-3d

cd openpose

cd models

getBaseModels.bat
