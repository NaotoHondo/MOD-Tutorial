# 2-1 KnosSDKの導入
# やること
KnosSDKをインストールし、車両諸元設定ファイルの展開と再構築の方法を学習する。
# KnosSDKとは？
>KN5(3Dファイル,テクスチャー)、ACD(車両設定データ)、BANK(音源データ)を再編集可能な形式へ変換・展開するためのツールです。
AssettoCorsaの挙動設定の仕組みを調べたい時や参考にしたい際にご利用ください。([ACJP LABS](http://labs.assettocorsa.jp/downloads/tools/kunossdk)より引用)

このツールはAssettoCorsa用に変換された3Dファイル、車両諸元設定ファイル、音源データファイルを編集可能な形式へ展開、、編集したファイルを再度AssettoCorsa用の形式に変換することができます。
このツールを利用してMODを作成していきます。  

# KnosSDKのインストール
1. [KnosSDKダウンロードサイト](http://labs.assettocorsa.jp/downloads/tools/kunossdk)へアクセスし、Download Japaneseの水色のボタンをクリックするとzipファイルのダウンロードが開始する。  
1. ダウンロードしたzipファイルを解凍し、フォルダ内にある`install.bat`を右クリックし、「管理者として実行」をクリックする。  
1. このアプリがデバイスに変更を加えることを許可しますか？と表示されるので、「はい」をクリックする。
1. インストール完了（アンインストールする際は`uninstall.bat`を同様に実行）  

# 車両諸元設定ファイルの展開
車両諸元設定ファイルを展開してみましょう。以下のディレクトリへ移動します。  
`C:\Program Files (x86)\Steam\steamapps\common\assettocorsa\content\cars`  
このディレクトリにはAssettoCorsa内の車両データが配置されています。MODファイルも最終的にはここに配置することでAssettoCorsaで読み込むことができます。  

では、例として`abarth500`のファイルを見てみましょう。`abarth500`フォルダの中に`data.acd`というファイルがあります。これがAssettoCorsa用に変換された車両諸元設定ファイルです。  
このファイルを右クリックして

