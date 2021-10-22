# 3Dモデルの作成
#### この章で作るもの
効率よく作業を進めるために，この章で作ったものを格納するためのフォルダを作成してください．ksEditor（3dモデルデータをassetto corsaにコンバートするためのソフト）でマテリアルやテクスチャを自動ロードするのにフォルダ構造が重要です．  
この章が終わるころには下のようなフォルダ構造になります．
![3Dモデル開発のフォルダ構造](https://user-images.githubusercontent.com/81402033/138374112-50e53019-490a-4ba5-bc23-c418ae2a3be2.png)
**texture**フォルダ　テクチャを入れるフォルダです．ksEditorはこのフォルダ名のフォルダからテクスチャを自動ロードするのでフォルダ名は正確につけてください．Texture texturesは×
**CarName.blend** blenderのファイルです．3Dモデルの作成はこのファイルで行います．
**CarName.blend1** blenderのバックアップファイル　拡張子の数字を消すとblendファイルとして開けるようになります．
**CarName.fbx** fbxファイル　blenderからエクスポートしたfbxファイルです．
**CarName.fbx.ini** ksEditor内のマテリアル設定がテキストファイル形式で保存されています．ksEditorでfbxを開くときにこのiniファイルからマテリアル設定がロードされるようになっています．  **
**CarName.kn5** assetto corsa専用の3Dモデルデータです.ksEditorでfbxからコンバートして作成します．
