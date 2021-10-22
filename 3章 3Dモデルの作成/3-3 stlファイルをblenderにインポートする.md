# やること
エクスポートしておいたstlファイルをblenderにインポートします。使用していたCADソフトの座標系によりインポート設定が変わる場合があります。

# インポート設定  
`blender`を起動して新規ファイルで`全般`を選択します。  
`ファイル`>`名前を付けて保存`で保存します。(筆者の場合はNK15)  
保存場所は作ったフォルダ内です．

`Aキー`でビューポート内のすべてのオブジェクトを選択し`Xキー`で削除
`Shift+C`で3Dカーソルを原点に配置します。（3Dカーソルの位置にモデルがインポートされるため）
`ファイル`>`インポート`>`stl`

![stlインポート1](https://user-images.githubusercontent.com/81402033/122321602-140a6380-cf5f-11eb-8c76-b0ab9d23a7cd.jpg)

## SOLIDWORKSの場合
右側`トランスフォーム`>`Zが前方`、`Yが上`に設定
`STLをインポート`をクリック。

![solidworksインポート設定](https://user-images.githubusercontent.com/81402033/122321537-f76e2b80-cf5e-11eb-862e-0b1d6e1e5e30.jpg)

## Creoの場合  
右側`トランスフォーム`>`スケール`を0.001に設定  
`Zが前方`、`Yが上`に設定
`STLをインポート`をクリック。  

![creoインポート設定](https://user-images.githubusercontent.com/81402033/122489249-28f7fd00-d01a-11eb-9ee2-01b08dd6e5f1.png)

## Autodesk Inventorの場合  
右側`トランスフォーム`>`Zが前方`、`Yが上`に設定
`STLをインポート`をクリック。  

![inventorインポート設定](https://user-images.githubusercontent.com/81402033/122489479-c6ebc780-d01a-11eb-9dd5-90bffffa77cc.png)

## Autodesk Fusion360の場合  
右側`トランスフォーム`>`スケール`を0.001に設定  
`Yが前方`、`Zが上`に設定
`STLをインポート`をクリック。  

![fusion360インポート設定](https://user-images.githubusercontent.com/81402033/122491593-3f548780-d01f-11eb-8c5a-7ee5793b5fbf.png)

以上で3-3 stlファイルをblenderにインポートする は終了です。  
次は [3-4 blenderアドオンを使用したリトポロジー](https://github.com/JSAE-ARCHIVES/MOD-Tutorial/blob/main/3%E7%AB%A0%203D%E3%83%A2%E3%83%87%E3%83%AB%E3%81%AE%E4%BD%9C%E6%88%90/3-4%20blender%E3%82%A2%E3%83%89%E3%82%AA%E3%83%B3%E3%82%92%E4%BD%BF%E7%94%A8%E3%81%97%E3%81%9F%E3%83%AA%E3%83%88%E3%83%9D%E3%83%AD%E3%82%B8%E3%83%BC.md) です。
