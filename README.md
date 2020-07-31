# QuestBasics

OculusQuest向けの基本的なサンプル、Gaze/Laser/コントローラ入力など
基本的な使い方がまとまっているサイトがみつからず、SDK付属のサンプルもわかりやすいとはいえないため、入門者向けにまとめてみました。

こんな基本機能の実装が見たい、という要望があればissueに挙げておいてください、
気が向いたら追加します（複雑なことはやりません、あくまでSDKの基本的な使い方）

リクエストが多いようなら、より詳細な実装のしかたはそのうちQiitaなどに書くかもしれません。

## 使用機器
* Oculus Quest（動作検証に使ったファームのバージョン　16.0.0.121）

## Unityバージョン
* 2019.2.21.f1  
2019.2系なら問題なく動くと思います  

## 使用ライブラリ
* Oculus Integration version18.0  
<https://developer.oculus.com/downloads/package/unity-integration/>

  プロジェクト内に同梱しています、
  以前は1.xxのようなバージョンの記述でしたが、最近のバージョンの記述は変わったようです

## 各シーンの概要
各シーンそれぞれ一つの機能しかないため理解しやすいと思います 
* _01_xx		いろいろなコントローラを表示  
* _02_xx		オブジェクトを操作する例  
* _03_xx		uGUIを操作する例  
* _04_xx		オブジェクト＋uGUIどちらも操作  
* _05_xx		コントローラーのいろいろな入力を取得  
* _06_xx		スティックの入力を利用する例  
* _07_xx		HMD側のセンサーの取得  

## 注意事項
* Githubにおいてあるものは、テクスチャ素材をLFSで管理していたので、ダウンロードするバージョンによってはzipでダウンロードするとテクスチャが含まれない可能性があります（Githubの仕様らしいです）
* その場合、Github Desktopをつかってプロジェクトを入手するか、以下のコマンドでcloneするとテクスチャ素材も入手できます。  
git clone https://github.com/hassydhw/OculusGoBasics.git
* ちなみにcloneでエラーが出る場合は git-lfsコマンドがちゃんとインストールされているか確認しましょう。

## ビルド時にエラーが出る場合
Oculusフォルダを削除し（Oculus Integrationがはいっているフォルダ）、アセットストアから、Oculus Ingegrationをダウンロードして取り込みなおしてみてください。
