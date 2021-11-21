# **3-2 CADからエクスポート**
# やること  
- CADソフトでモデリングした車両モデルを3DCG系ソフトで扱えるようにするために、3Dモデルの一般的な形式(.stl)に変換してエクスポートします。  
- エクスポートでCADモデルがポリゴンに変換される際に最もポリゴン数が少なくなるよう、エクスポート設定を変更する必要があります。  
- エクスポート先はCarNameフォルダです。
# 用語解説
## CADソフト
>ソリッドモデリング（英: Solid modeling）またはソリッドモデル（英語: Solid model）とは、3次元コンピュータグラフィックスにおいて、体積を持った（中身の詰まった）3次元構造、またはそれらを作成する目的のモデリング体系のことである。（[Wikipedia](https://ja.wikipedia.org/wiki/%E3%82%BD%E3%83%AA%E3%83%83%E3%83%89%E3%83%A2%E3%83%87%E3%83%AA%E3%83%B3%E3%82%B0)より引用）
## 3DCG系ソフト
>サーフェスモデルまたはサーフェスモデリングとは、3DCGにおいて、表面のみが定義された3次元構造、またはそれらを作成する目的のモデリング体系のことである。サーフェスモデルは中身が詰まっていないため、しばしば張り子、張りぼてとも形容される。レンダリングにより画像を生成することが主目的の一般的な3DCGソフトウェアにおいては、おそらく最もよく使われる方式である。（[Wikipedia](https://ja.wikipedia.org/wiki/%E3%82%B5%E3%83%BC%E3%83%95%E3%82%A7%E3%82%B9%E3%83%A2%E3%83%87%E3%83%AA%E3%83%B3%E3%82%B0)より引用）
# 用意するもの
- 各チームで使用しているCADソフト  
- 車両のフルアセンブリCADモデル

# エクスポート設定
### SOLIDWORKS  
- `ファイル>指定保存` からファイルの種類`.stl`を選択。  
- `オプション`を開く。  
- 単位を`m`に設定する。  
- 解像度を粗表示にする。  
![SOLIDWORKSエクスポート1](https://user-images.githubusercontent.com/81402033/122487977-74f57280-d017-11eb-8f25-f9aef1cc626f.jpg)
![solidworksエクスポート設定](https://user-images.githubusercontent.com/81402033/142764722-4096aec9-2d8a-4178-b2e5-1844f97669a8.png)


___
### Creo  
- `ファイル`>`名前を付けて保存`>`コピーを保存`からタイプ`.stl`を選択。  
- `オプション`を開く。    
- 解像度を最低設定にする  
![creoエクスポート設定1](https://user-images.githubusercontent.com/81402033/122488123-c7cf2a00-d017-11eb-88d6-8f6118b37324.jpg)
![creoエクスポート設定2](https://user-images.githubusercontent.com/81402033/122488127-c9005700-d017-11eb-9fa6-897d9996d842.jpg)

___
### Autodesk Inventor  
- `ファイル`>`書き出し`>`CAD形式`からファイルの種類`.stl`を選択。
- `オプション`を開く。  
- 単位を`m`に設定する。  
- 解像度を最低にする。  
![inventorエクスポート設定1](https://user-images.githubusercontent.com/81402033/122487989-7c1c8080-d017-11eb-950c-296e27f9d10a.jpg)
![inventorエクスポート設定2](https://user-images.githubusercontent.com/81402033/122487993-7de64400-d017-11eb-8537-a356381aa5ee.jpg)
![inventorエクスポート設定3](https://user-images.githubusercontent.com/81402033/122487996-7fb00780-d017-11eb-90b9-88d96870fa51.jpg)

___
### Autodesk Fusion360
- `ファイル`>`3Dプリント`  
- 右側3Dプリントタブで`選択`、`メッシュを...`にチェック  
- 3Dビューポート内でメッシュを選択する。  
- リファインメントオプションで解像度を最低にする。
![fusion360エクスポート設定](https://user-images.githubusercontent.com/81402033/122695384-2cd68a00-d27b-11eb-9547-592136f9b100.png)
![fusion360エクスポート設定2](https://user-images.githubusercontent.com/81402033/122695392-306a1100-d27b-11eb-937d-1841fe562e75.png)

___
以上で 3-2 CADからエクスポート は終了です。

| Back | Next |
|:---:|:---:|
| [3-1 フォルダ作成](https://github.com/JSAE-ARCHIVES/MOD-Tutorial/blob/main/3%E7%AB%A0%203D%E3%83%A2%E3%83%87%E3%83%AB%E3%81%AE%E4%BD%9C%E6%88%90/3-1%20%E3%83%95%E3%82%A9%E3%83%AB%E3%83%80%E4%BD%9C%E6%88%90.md) | [3-3 blenderの導入](https://github.com/JSAE-ARCHIVES/MOD-Tutorial/blob/main/3%E7%AB%A0%203D%E3%83%A2%E3%83%87%E3%83%AB%E3%81%AE%E4%BD%9C%E6%88%90/3-3%203D%E3%83%A2%E3%83%87%E3%83%AA%E3%83%B3%E3%82%B0%E3%82%BD%E3%83%95%E3%83%88(blender)%E3%81%AE%E5%B0%8E%E5%85%A5.md) |

