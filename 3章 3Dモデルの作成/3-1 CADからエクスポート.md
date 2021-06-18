# 3-1でやること  
CADソフトでモデリングした車両モデルを3DCG系ソフトで扱えるようにするために、3Dモデルの一般的な形式(.stl)に変換してエクスポートします。
# 用語解説
## CADソフト
>ソリッドモデリング（英: Solid modeling）またはソリッドモデル（英語: Solid model）とは、3次元コンピュータグラフィックスにおいて、体積を持った（中身の詰まった）3次元構造、またはそれらを作成する目的のモデリング体系のことである。（[Wikipedia](https://ja.wikipedia.org/wiki/%E3%82%BD%E3%83%AA%E3%83%83%E3%83%89%E3%83%A2%E3%83%87%E3%83%AA%E3%83%B3%E3%82%B0)より引用）
## 3DCG系ソフト
>サーフェスモデルまたはサーフェスモデリングとは、3DCGにおいて、表面のみが定義された3次元構造、またはそれらを作成する目的のモデリング体系のことである。サーフェスモデルは中身が詰まっていないため、しばしば張り子、張りぼてとも形容される。レンダリングにより画像を生成することが主目的の一般的な3DCGソフトウェアにおいては、おそらく最もよく使われる方式である。（[Wikipedia](https://ja.wikipedia.org/wiki/%E3%82%B5%E3%83%BC%E3%83%95%E3%82%A7%E3%82%B9%E3%83%A2%E3%83%87%E3%83%AA%E3%83%B3%E3%82%B0)より引用）
# 用意するもの
- 各チームで使用しているCADソフト  
- 車両のフルアセンブリモデル

# エクスポート設定
## SOLIDWORKS
`ファイル>指定保存` からファイルの種類`.stl`を選択。  
下の`オプション`を開き、単位を`m`に設定する。  
![SOLIDWORKSエクスポート1](https://user-images.githubusercontent.com/81402033/122487977-74f57280-d017-11eb-8f25-f9aef1cc626f.jpg)
![SOLIDWORKSエクスポート2](https://user-images.githubusercontent.com/81402033/122487979-76bf3600-d017-11eb-854a-5c7fc2c9ca1b.jpg)

___
## Creo  
`ファイル`>`名前を付けて保存`>`コピーを保存`からタイプ`.stl`を選択。
![creoエクスポート設定1](https://user-images.githubusercontent.com/81402033/122488123-c7cf2a00-d017-11eb-88d6-8f6118b37324.jpg)
![creoエクスポート設定2](https://user-images.githubusercontent.com/81402033/122488127-c9005700-d017-11eb-9fa6-897d9996d842.jpg)


___
## Autodesk Inventor  
`ファイル`>`書き出し`>`CAD形式`からファイルの種類`.stl`を選択。
`オプション`を開き、単位を`m`に設定する。  
![inventorエクスポート設定1](https://user-images.githubusercontent.com/81402033/122487989-7c1c8080-d017-11eb-950c-296e27f9d10a.jpg)
![inventorエクスポート設定2](https://user-images.githubusercontent.com/81402033/122487993-7de64400-d017-11eb-8537-a356381aa5ee.jpg)
![inventorエクスポート設定3](https://user-images.githubusercontent.com/81402033/122487996-7fb00780-d017-11eb-90b9-88d96870fa51.jpg)

___
## Autodesk Fusion360
以上で`3-1 CADからエクスポート`は終了です。
次は [3-2 blenderの導入](https://github.com/JSAE-ARCHIVES/MOD-Tutorial/blob/main/3%E7%AB%A0%203D%E3%83%A2%E3%83%87%E3%83%AB%E3%81%AE%E4%BD%9C%E6%88%90/3-2%203D%E3%83%A2%E3%83%87%E3%83%AA%E3%83%B3%E3%82%B0%E3%82%BD%E3%83%95%E3%83%88(blender)%E3%81%AE%E5%B0%8E%E5%85%A5.md) です。
