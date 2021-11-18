# **2-11 lods.iniの設定**   
# やること
アセットコルサでは、`C:\Program Files (x86)\Steam\steamapps\common\assettocorsa\content\cars\○○\date`にある`lods.ini`で表示するモデルのディティールを設定しています。

# 用語解説
### LODとは？

>「LOD」とは、「Level of Detail」の略であり、直訳すると「細かさの度合い」を意味しています。カメラからの距離に応じモデルのポリゴン数を制御することで、シーンの計算負荷を軽減する方法です。
3Dで描画されるキャラクターなどは、基本的にポリゴン数やテクスチャーの数、サイズ等が豊富であればあるほど高い精度での実現ができますが、その反面、データが重くなります。このような負荷を軽減する目的としてLODを活用することで、画面上での見え方を調整しながら最適なデータ容量での表示を行い、見た目を大きく損なわずに処理を高速化することが可能となります。ゲームのリアルタイムレンダリングで使われることが多いです。([デジタルハリウッドスクールHP](https://school.dhw.co.jp/course/3dcg/contents/w_lod.html)より引用)  

HR : High Resolution 高解像度
LR : Low Resolution 低解像度

通常であればポリゴン数の異なるモデルを複数用意して設定をしますが、このチュートリアルでは簡単のために高解像度モデルのみを使用します。


# ファイルの構成
### lod.iniファイルの構成
`[COCKPIT_HR]`  
  +　コックピットの表示設定  


`[DRIVER_HR]`  
  + ドライバーの表示設定  

`[LOD_0]`
 +　表示するモデルのファイル名とカメラからの距離を指定。


`[LOD_1~3]`  
  + モデルの表示をカメラ距離に応じて分けるならここを設定。今回はどの距離でも同じモデルを表示するので削除。
 

# 作業内容
### LODの設定
1. `C:\Program Files (x86)\Steam\steamapps\common\assettocorsa\content\cars\○○\date`にある`lods.ini`を開く　　
2. `[COCKPIT_HR]`と`[DRIVER_HR]`の`DISTANCE_SWITCH=`で高解像度モデルを表示する距離を指定。基本的に弄らなくてよい。
3. `[LOD_0]`の`FILE=`で表示するkn5モデルのファイル名を指定。
4. `[LOD_0]`の`IN=`を0、`OUT=`を2000に設定。inは表示開始される距離、outは表示終了する距離。
6. `[LOD_1]`以降は低解像度モデルがない場合は削除する。


以上で[2-11 lods.iniの設定](https://github.com/JSAE-ARCHIVES/MOD-Tutorial/blob/main/2%E7%AB%A0%20%E8%BB%8A%E4%B8%A1%E8%AB%B8%E5%85%83%E3%81%AE%E8%A8%AD%E5%AE%9A/2-08%20%E3%82%A8%E3%83%B3%E3%82%B8%E3%83%B3%E3%81%AE%E8%A8%AD%E5%AE%9A.md)は終了です。  
お疲れ様でした。  

| Back | Next |
|:---:|:---:|
| [2-08 エンジンの設定](https://github.com/JSAE-ARCHIVES/MOD-Tutorial/blob/main/2%E7%AB%A0%20%E8%BB%8A%E4%B8%A1%E8%AB%B8%E5%85%83%E3%81%AE%E8%A8%AD%E5%AE%9A/2-08%20%E3%82%A8%E3%83%B3%E3%82%B8%E3%83%B3%E3%81%AE%E8%A8%AD%E5%AE%9A.md) | [2-12 サスペンションの設定](https://github.com/JSAE-ARCHIVES/MOD-Tutorial/blob/main/2%E7%AB%A0%20%E8%BB%8A%E4%B8%A1%E8%AB%B8%E5%85%83%E3%81%AE%E8%A8%AD%E5%AE%9A/2-09%20%E3%82%B5%E3%82%B9%E3%83%9A%E3%83%B3%E3%82%B7%E3%83%A7%E3%83%B3%E3%81%AE%E8%A8%AD%E5%AE%9A.md) |
