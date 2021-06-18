# 2-3 車両諸元ファイルの展開
# やること
[2-1 KnosSDKの導入](https://github.com/JSAE-ARCHIVES/MOD-Tutorial/blob/main/2%E7%AB%A0%20%E8%BB%8A%E4%B8%A1%E8%AB%B8%E5%85%83%E3%81%AE%E8%A8%AD%E5%AE%9A/2-1%20KnosSDK%E3%81%AE%E3%82%A4%E3%83%B3%E3%82%B9%E3%83%88%E3%83%BC%E3%83%AB.md)でインストールしたKnosSDKを利用して車両諸元設定ファイルを展開・再変換をする。  

# 車両諸元ファイルの展開
KnosSDKを利用して車両諸元ファイルを展開してみましょう。以下のディレクトリへ移動します。  
`C:\Program Files (x86)\Steam\steamapps\common\assettocorsa\content\cars`  
このディレクトリにはAssettoCorsa内の車両データが配置されています。MODファイルも最終的にはここに配置することでAssettoCorsaで読み込むことができます。  

では、例として`abarth500`のファイルを見てみましょう。`abarth500`フォルダの中に`data.acd`というファイルがあります。これがAssettoCorsa用に変換された車両諸元設定ファイルです。  
このファイルを右クリックして「展開」をクリックします。  

すると「data」フォルダが作成されます。このフォルダに全ての車両諸元設定ファイルが展開されます。 

展開することで車両諸元を編集することができるようになります。

# 車両諸元設定ファイルの再変換
「data」フォルダを右クリックして「KsACDにコンパイル」を選択します。すると`data.acd`ファイルが作成され、AssettoCorsaで読み込むことができるようになります。

# dataフォルダ内の車両諸元設定ファイルの説明
最小構成
| ファイル名 | 機能 | 参照ファイル | 作業番号 |  
----|---- |---- |---- 
aero.ini                | エアロデバイスの設定 | wing_body_AOA_CD.lut / wing_body_AOA_CD.lut |2-4
wing_body_AOA_CD.lut    | 抗力係数のデータ ||
wing_body_AOA_CL.lut    | 揚力係数のデータ ||
brakes.ini              | ブレーキの設定 ||
cameras.ini             | カメラ位置の設定 ||
car.ini                 | 車両全般の設定
colliders.ini           | 衝突モデルの座標設定 ||
dash_cam.ini            | ダッシュボードカメラの設定 ||
driver3d.ini            | ドライバーモデルの設定 ||
drivetrain.ini          | ドライブトレインの設定 ||
engine.ini              | エンジンの設定 | power.lut |
power.lut               | トルクカーブのデータ     
throttle.lut            | スロットル開度のデータ
lods.ini                | 車両モデルの表示設定
setup.ini               | マシンセッティングの設定
suspention.ini          | サスペンションの設定
tyres.ini               | タイヤの設定 | F3hard_front.lut / F3hard_rear.lut / tcurve_F3hard.lut|
F3hard_front.lut        | フロントタイヤ温度のデータ||
F3hard_rear.lut         | リヤタイヤの温度データ||
tcurve_F3hard.lut       | タイヤカーブのデータ||

追加設定ファイル（FOR_LATER_USE）
| ファイル名 | 機能 | 参照ファイル | 作業番号 |  
----|---- |---- |---- 
ai.ini                  | 
ambient_shadows.ini     | 
analog_instruments.ini  |  
blurred_objects.ini     | 
damage.ini              | 
digital_instruments.ini |  
drs.ini  
electronics.ini  
escmode.ini  
final.rto  
flame_presets.ini  
flames.ini  
height_diffuser_CD.lut  
height_diffuser_CL.lut  
height_frontwing_CD.lut  
height_frontwing_CL.lut  
fuel_cons.ini  
lights.ini  
mirrors.ini  
proview_nodes.ini  
ratios.rto  
sounds.ini  
suspention_graphics.ini  
wing_animation.ini  
wing_controller_brake.lut  
wing_controller_speed.lut  
wing_diffuser_AOA_CD.lut  
wing_diffuser_AOA_CL.lut  
wing_front_AOA_CD.lut  
wing_front_AOA_CL.lut  
wing_resr_AOA_CD.lut  
wing_rear_AOA_CL.lut  
wing_rearmovable_AOA_CD.lut  
wing_rearmovable_AOA_CL.lut  