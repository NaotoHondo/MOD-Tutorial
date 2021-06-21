# MODとは？
>あるゲームのグラフィックや様々なデータを改造するプログラムやファイルのこと。MODを導入することによってそのゲームを改造・変更（Modification）し、そのゲームのグラフィックエンジンや物理エンジンなどの基本システムを用いつつ、本編とは別のシナリオやグラフィック、モデル、システムで遊べるようになる。単にMODと呼ばれるものの場合、大抵は有志（そのゲームのファン）ベースで制作されるものを意味する。MOD制作者は作りたいMODの目的に応じて3Dグラフィック制作ソフト、ペイントソフト、スクリプトを組むためのテキストソフトなどを活用し、目的のMODを作っていく。（[Wikipediaより引用](https://ja.wikipedia.org/wiki/Mod_(%E3%82%B3%E3%83%B3%E3%83%94%E3%83%A5%E3%83%BC%E3%82%BF%E3%82%B2%E3%83%BC%E3%83%A0))）

# AssettoCorsa車両MODの構造
基本的には  
- グラフィック（3Dモデル, テクスチャ）のファイル（**.kn5**, .dds, .png, .ksanim）  
- 車両諸元のテキストファイル（**.acd**, .ini, .lut, .json, .knh）  
- サウンドのファイル（.bank）   

で構成されている。  

AssettoCorsaのMOD作成においてはこれらのファイルを用意し、適切なフォルダに配置することでゲーム上で動作するようになる。

詳しいフォルダ構造は以下のようになっている

CARNAME   
　├ animations/  
　│　└ steer.ksanim  
　├ sfx/  
　│　└ CARNAME.bank  
　├ skins/  
　│　└ CARNAME/  
　│　　　├ GOMMA_BASE_dirt3.dds  
　│　　　├ livery.png  
　│　　　├ preview.jpg  
　│　　　├ protection.dds  
　│　　　├ SkinBase.dds   
　│　　　└ ui_skin.json  
　├ texture/  
　│　└ N/A   
　├ ui/  
　│　├ badge.png  
　│　├ preview_small.png  
　│　└ ui_car.json  
　├ body_shadow.png  
　├ collider.kn5  
　├ data.acd  
　├ driver_base_pos.knh    
　├ logo.png  
　├ CARNAME.kn5  
　├ tyre_0_shadow.png  
　├ tyre_1_shadow.png  
　├ tyre_2_shadow.png  
　└ tyre_3_shadow.png  
 
2章 車両諸元の設定 では、 data.acdファイルを展開、諸元設定用のテキストファイル（.ini, .lut）の編集、data.acdファイルへの再構築の方法を解説する。  

3章 3Dモデルの作成 では、3Dモデル（.kn5）の作成、テクスチャ（.dds, .png）の作成の方法を解説する。  

4章 MODパッケージング では、ゲーム内で表示されるロゴやプレビューの設定など、最終的なパッケージングの作業を解説する。
