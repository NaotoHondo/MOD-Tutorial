# リトポロジーとは？
モデル形状を維持したままポリゴン数を減らしてメッシュを再構築することをリトポロジーといいます。  
CADからエクスポートしたメッシュデータは細かく（数百万△ポリゴン）重たいデータですので、Assetto Corsaで動かすために3Dモデルを30万△ポリゴン以内に収める必要があります。  
配布中のNK16 MODでは完全手動でリトポロジーを行いました（blenderで一からモデリングしたに等しい）。3DCGのテクニックが要求されることに加えて非常に時間がかかる（約2か月）ので、リトポロジーの自動化ツール（Quad Remesher）も併用して少しでも手間を減らせるようにしましょう。

# QuadRemesherのダウンロード  
[QuadRemesherの解説（外部サイト）](https://www.youtube.com/watch?v=IUoaDVSq7ks)  

[Quad Remesher](https://exoside.com/quadremesher/)公式サイトにアクセスし、Download TRIALを押す。
![Quadremesher導入1](https://user-images.githubusercontent.com/81402033/122494242-fbb04c80-d023-11eb-80bf-80b29b7674ce.png)
必要事項を記入する。  
![Quadremesher導入3](https://user-images.githubusercontent.com/81402033/122494346-28fcfa80-d024-11eb-8ce0-a8e114dc8f20.png)
確認メールのリンクにアクセスしてBlender addonをクリックするとzipファイルが自動でダウンロードされる。  
![Quadremesher導入4](https://user-images.githubusercontent.com/81402033/122496551-ebe63780-d026-11eb-9814-57ec5d2da83a.png)

# Quad Remesherをblender上で有効化する  
`編集`>`プリファレンス`>`アドオン`>`インストール`>ダウンロードしたzipファイル(zipのままでOK)>`アドオンのインストール`  
![Quadremesher導入5](https://user-images.githubusercontent.com/81402033/122497580-872bdc80-d028-11eb-9001-ef4adb8a76f6.png)  
Quad Remesherアドオンにチェックをつけて左下から`プリファレンスを保存`  
![Quadremesher導入6](https://user-images.githubusercontent.com/81402033/122497795-f275ae80-d028-11eb-9629-167f0ec1d135.png)  
blender3Dビューポート上にカーソルを置きNキーでプロパティシェルフを展開する。  
プロパティシェルフにQuad Remeshのタブができているのでそこをクリック。  
![Quadremesher導入7](https://user-images.githubusercontent.com/81402033/122498285-cdce0680-d029-11eb-819a-1d6e88417aff.png)  

オブジェクトを一つ選択し`REMESH IT`をクリックすると初回はライセンス認証を求められるのでダウンロード時に記入したEmailを記入し左のStrat TRIALをクリック  

以上でQuad Remesherの導入は完了です。
### QuadRemesherの使い方
`Quad Count`  
目標とする四角ポリゴン数（あくまで目安です。）  
`Quad Size Settings`
ハイポリモデルのディティールをどこまで再現するか（曲率が高い部分にポリゴン数を割くかどうか）  
数字が高いほど解像度の高いリトポロジーが行えるが、ポリゴン数をあまり削減できなくなるのでお好みで数字をいじってみてください。

# 作業1 オブジェクトの分割、削除
インポートしたモデルはすべてのパーツが一つのオブジェクトにまとまってしまっている。Quad Remesherはオブジェクト単位でリトポロジーを行うので、一つのオブジェクトに含まれるパーツが多すぎると負荷が高く固まってしまう。そこでリトポロジーの前段階としてオブジェクトをパーツごとに分けていく作業を行う必要がある。
`L`で選択できるひとつながりになったメッシュを別オブジェクトとして切り離していくイメージ。  
左右で同じパーツがあるものは片方削除する。リトポロジー後にミラーで複製する。
オブジェクトモードでモデルを選択した状態で`Tab`でエディットモードにする（頂点数が多いとここで急に重たくなる）  
パーツにカーソルを合わせて`L`でひとつながりのメッシュを選択することができる。
オブジェクトを分けたいパーツを選択したら`P`>`選択`でオブジェクトを分離する。
これを繰り返す。

フォルダを作成する
デスクトップ上に車両の名前フォルダを作成する。今後の3Dモデル作成作業はこのフォルダ内で行う。
**注意　ディレクトリには2バイト文字を含まないようにしてください[KsEditoeにインポート](https://github.com/JSAE-ARCHIVES/MOD-Tutorial/blob/main/3%E7%AB%A0%203D%E3%83%A2%E3%83%87%E3%83%AB%E3%81%AE%E4%BD%9C%E6%88%90/KsEditor%E3%81%AB%E3%82%A4%E3%83%B3%E3%83%9D%E3%83%BC%E3%83%88.md)する際にエラーを生じる可能性があります。**  
blenderで新規ファイルを作成する
`ファイル`>`名前を付けて保存`>**車両の名前**  
`A`で全選択、`X`で削除  
`ファイル`>`インポート`>`stl`で[エクスポートしたstlファイルを開く。](https://github.com/JSAE-ARCHIVES/MOD-Tutorial/blob/main/3%E7%AB%A0%203D%E3%83%A2%E3%83%87%E3%83%AB%E3%81%AE%E4%BD%9C%E6%88%90/3-3%20stl%E3%83%95%E3%82%A1%E3%82%A4%E3%83%AB%E3%82%92blender%E3%81%AB%E3%82%A4%E3%83%B3%E3%83%9D%E3%83%BC%E3%83%88%E3%81%99%E3%82%8B.md)  
インポートした車両がblender原点にない場合
`G`>`X`、`Y`、`Z`で位置を合わせる。(目分量)  
`オブジェクト`>`適用`>`全トランスフォーム`でオブジェクトの座標が3D空間の原点にリセットされる。










