# gammaCorrCS.exe


## English

### Overview
gammaCorrCS.exe is a high‑speed gamma‑correction tool built with DirectX 11 Compute Shaders.
It performs tone‑curve based gamma correction on large images with GPU acceleration.
The application uses Direct3D for rendering and provides smooth interaction for previewing results.


## Features
- Tone‑curve based gamma correction (GPU accelerated)
- Supported formats: JPG / BMP / PNG / TIFF / standard RAW
- Maximum loadable image size: 16000 × 16000 pixels  
- (Larger images are automatically resized)
- Mouse‑wheel zoom and viewpoint movement
- Mouse‑drag scrolling
- Format conversion and saving


## Development Environment
- Windows 11
- Visual Studio 2022 (VC++ / MFC)
- GPU with DirectX 11 support required


## Class Structure
- CgammaCorrCSDlg — MFC main dialog
- CbuttonDlg — Button UI class
- CeditImgDlg — Parameter editor class
- Cdx11 — DirectX 11 initialization, rendering, compute shader setup & execution
- CWICTextureLoader — Image loading class

## Build Instructions
- Open the solution in Visual Studio 2022 or later.
- Configuration: Release/x64 or Debug/x64
- MFC: Use MFC in a Shared DLL
- Code Generation: /MD (Multithreaded DLL)
- Note: Using /MT (Static) will conflict with MFC and the project will not build.




## 日本語

## プログラムの概要

DirectX11のコンピュート・シェーダー（CS）を利用して、高速で画像のガンマ補正を 行います。
DirectX3Dを使用します。

##主な機能
- トーンカーブによる、ガンマ補正
- 対応フォーマットは、jpg,bmp,png,tif,標準的なRAW
- ロード可能画像サイズ、16000×16000pixel
- マウスホイールによるズーム、視点移動
- マウスドラッグによる、スクロール
- フォーマット変換セーブ

対応画像フォーマットは、jpg / bmp / png / tif（サイズは16000×16000pixelまで）。
それ以上の画像は、自動でリサイズされます。



## 開発環境

- Windows 11
- Visualstudio 2022    VC++ MFC
- GPUがDirectX11をサポートしている必要があります


## クラス

- CgammaCorrCSDlg　MFCメイン
- CbuttonDlg　　　　ボタンクラス
- CeditImgDlg　　　　エディター（パラメーター作成）クラス
- Cdx11　　　　　　　DirectC11のイニシャライズ、描画、コンピュートシェーダーのイニシャライズ、実行クラス
- CWICTextureLoader　画像ローダークラス



## 【ビルド方法】
- Visual Studio 2022 以降で開きます。
- 構成：Release / x64　または　Debug/x64
- MFC：Use MFC in a Shared DLL（共有DLL）
- コード生成：/MD（マルチスレッドDLL）
- ※ /MT（スタティック）にすると MFC と衝突してビルドできません。



