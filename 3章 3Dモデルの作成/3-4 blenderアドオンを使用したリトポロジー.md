# リトポロジーとは？
モデル形状を維持したままポリゴン数を減らしてメッシュを再構築することをリトポロジーという。  
CADからエクスポートしたメッシュデータは細かく（数百万△ポリゴン）重たいデータになっている。Assetto Corsaで動かす3Dモデルは30万△ポリゴン以内に収める必要がある。  
配布中のNK16 MODでは完全手動でリトポロジーを行ったが3DCGのテクニックが要求されることに加えて非常に時間がかかる（約2か月）ので、リトポロジーの自動化ツールを活用する。

# QuadRemesherのダウンロード  
[Quad Remesher](https://exoside.com/quadremesher/)公式サイトに飛び、Download TRIALを押す。
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

# 作業1 オブジェクトを分割する
インポートしたモデルはすべてのパーツが一つのオブジェクトにまとまってしまっている。Quad Remesherはオブジェクト単位でリトポロジーを行うので、一つのオブジェクトに含まれるパーツが多すぎると負荷が高く固まってしまう。そこでリトポロジーの前段階としてオブジェクトをパーツごとに分けていく作業を行う必要がある。  
パーツごとといってもCADの時と同じレベルで分ける必要はない。Assetto Corsa内で動くパーツで分けるくらいの感覚でOK。
### オブジェクト分割の例

フォルダを作成する
デスクトップ上に車両の名前フォルダを作成する。今後の3Dモデル作成作業はこのフォルダ内で行う。
**注意　ディレクトリには2バイト文字を含まないようにしてください[KsEditoeにインポート](https://github.com/JSAE-ARCHIVES/MOD-Tutorial/blob/main/3%E7%AB%A0%203D%E3%83%A2%E3%83%87%E3%83%AB%E3%81%AE%E4%BD%9C%E6%88%90/KsEditor%E3%81%AB%E3%82%A4%E3%83%B3%E3%83%9D%E3%83%BC%E3%83%88.md)する際にエラーを生じる可能性があります。**  
blenderで新規ファイルを作成する
`ファイル`>`名前を付けて保存`>**車両の名前**  
`A`で全選択、`X`で削除  
`ファイル`>`インポート`>`stl`で[エクスポートしたstlファイルを開く。](https://github.com/JSAE-ARCHIVES/MOD-Tutorial/blob/main/3%E7%AB%A0%203D%E3%83%A2%E3%83%87%E3%83%AB%E3%81%AE%E4%BD%9C%E6%88%90/3-3%20stl%E3%83%95%E3%82%A1%E3%82%A4%E3%83%AB%E3%82%92blender%E3%81%AB%E3%82%A4%E3%83%B3%E3%83%9D%E3%83%BC%E3%83%88%E3%81%99%E3%82%8B.md)  
インポートした車両がblender原点にない場合
`G`>`X`、`Y`、`Z`で位置を合わせる。(目分量)  
`Shift+C`で3Dカーソルを原点に戻した後、`オブジェクト`>`原点を設定`>`原点を3Dカーソルへ移動`
オブジェクトモードでモデルを選択した状態で`Tab`でエディットモードにする（頂点数が多いとここで急に重たくなる）








