### UV展開とは？
>UV展開とは、3次元の情報であるメッシュを展開し、2次元の座標に対応させる作業をいいます。 組み上げたペーパークラフトの模型を平面に戻す作業のようなもの、と考えていいと思います。
[UV展開の基本](https://www.tomog-storage.com/entry/2018/08/16/225608)

上記の基本的なUV展開はテクスチャをしっかり書き込む際には重要ですが，UV展開とテクスチャ作成にこだわると膨大な時間がかかるので，ここでは非常に簡易的な方法を紹介します．テクスチャでディテールを描き込むことはせず，パーツは単色ベタ塗りにすることで手間を減らし軽量なデータにすることができます．

# 3.簡易的なUV展開
UV Editingワークスペースで作業します．画面左側がUV座標系で画面右側が3Dビューポートです．
![UV展開ワークスペース](https://user-images.githubusercontent.com/81402033/138378919-6d06fae4-5592-4c86-8280-8a5edda46b4c.png)
右側の3Dビューポート上でUV展開したいオブジェクトを選択して編集モードに入り，選択して`Uキー`>`ビューから投影`でUV展開  
`Sキー`(拡縮)，`Gキー`(移動)等を使ってタイル画像上の任意の色タイル上にUVを移動させる．  
![UV展開前](https://user-images.githubusercontent.com/81402033/138379124-1541e7f3-0043-41f1-b6fa-880642696f16.png)
![UV展開](https://user-images.githubusercontent.com/81402033/138379128-311cacd5-e31d-4b1b-b5af-be32ee374d12.png)


| Back | Next |
|:---:|:---:|
| [3-7 マテリアル作成](https://github.com/JSAE-ARCHIVES/MOD-Tutorial/blob/main/3%E7%AB%A0%203D%E3%83%A2%E3%83%87%E3%83%AB%E3%81%AE%E4%BD%9C%E6%88%90/3-7%20%E3%83%9E%E3%83%86%E3%83%AA%E3%82%A2%E3%83%AB%E4%BD%9C%E6%88%90.md) | [3-9 ダミー配置と親子付け](https://github.com/JSAE-ARCHIVES/MOD-Tutorial/blob/main/3%E7%AB%A0%203D%E3%83%A2%E3%83%87%E3%83%AB%E3%81%AE%E4%BD%9C%E6%88%90/3-9%20%E3%83%80%E3%83%9F%E3%83%BC%E9%85%8D%E7%BD%AE%E3%81%A8%E8%A6%AA%E5%AD%90%E4%BB%98%E3%81%91.md) |

