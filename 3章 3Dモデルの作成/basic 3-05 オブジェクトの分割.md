# 3-5 オブジェクトの分割

# オブジェクトを分割する意味
- CADからインポートした車両は一つのオブジェクト内にすべての頂点が含まれている状態になっています。
- Assetto Corsaでは、1つのオブジェクトが含むことができる頂点数に上限があります。（1オブジェクトにつき2万程度）
- 1つのオブジェクトに含まれる頂点数が制限内に収まるよう適当なパーツごとにオブジェクトを分割する必要があります。
- ホイールやステアリングなどのゲーム内で動く部品は、オブジェクト単位で動くようになっているので、パーツごとにオブジェクトを分割していく必要があります。
## オブジェクト分割の基準
オブジェクトを分割するにあたって、分け方が決まっているパーツがあります。  
- assettocorsa上で動きがある部品
  - タイヤ類（タイヤ/ホイール/ハブ/ブレーキディスク等のタイヤと一緒に開店するパーツ）は一つのオブジェクトとしてまとめます（4輪分で4オブジェクト）  
  - ハブ　AssettoCorsa上で地面の凹凸、転舵などで動きます。（4輪分で4オブジェクト）  
  - ステアリング AssettoCorsa上でステアリング操作で動きます。回転軸は一つしかないのでユニバーサルジョイント手前までの部品を1オブジェクトとしてまとめます。  
- 次の工程（頂点数の削減）がうまくいくようにするためにやっておくべき分割  
  - 薄板系のパーツ（カウルやエアロ、パイプでできたフレーム等）はそれぞれ別オブジェクトにしておきます。  
- その他  
  - 基本的に自由です。1オブジェクトが2万頂点を超えないように（余裕をもって）パーツごとに分割します。  
## 分割作業
1. オブジェクトモードでモデルを選択した状態で`Tab`でエディットモードにする（頂点数が多いとここで急に重たくなる）
1. `L`でひとつながりになったメッシュを選択し、`P`>`選択`で別オブジェクトとして切り離していく。   
これを繰り返す。

### 3Dモデルのチェック
Blender上では表示されているが，3DCGでは基本的に裏面は描画されない．気づかないうちに面が裏返っているとassettocorsaにもっていったときにパーツが透明になっていたり表示（陰影）がおかしくなってしまう．
#### 面の向きの確認
- ビューポートオーバーレイの設定パネルを開き`面の向き`にチェック  
- 表面が青，裏面が赤で表示される．  
- 面が裏返ってしまっているオブジェクトがあったら，編集モードで選択して`Shift+N`で法線を再計算すると直ることが多い．  
- 直らない場合は法線を再計算タブの中の`内側に`にチェック．  
- これでもうまくいかない場合は裏返ってる面を個別に選択して`Alt+N`，`反転`で修正する．
![面の向きの表示](https://user-images.githubusercontent.com/81402033/138587895-65162c80-0fd5-4077-ab3a-dd5638d09684.png)


| Back | Next |
|:---:|:---:|
| [3-4 stlファイルをblenderにインポートする](https://github.com/JSAE-ARCHIVES/MOD-Tutorial/blob/main/3%E7%AB%A0%203D%E3%83%A2%E3%83%87%E3%83%AB%E3%81%AE%E4%BD%9C%E6%88%90/3-4%20stl%E3%83%95%E3%82%A1%E3%82%A4%E3%83%AB%E3%82%92blender%E3%81%AB%E3%82%A4%E3%83%B3%E3%83%9D%E3%83%BC%E3%83%88%E3%81%99%E3%82%8B.md) | [3-6 テクスチャ作成](https://github.com/JSAE-ARCHIVES/MOD-Tutorial/blob/main/3%E7%AB%A0%203D%E3%83%A2%E3%83%87%E3%83%AB%E3%81%AE%E4%BD%9C%E6%88%90/3-6%20%E3%83%86%E3%82%AF%E3%82%B9%E3%83%81%E3%83%A3%E4%BD%9C%E6%88%90.md) |












