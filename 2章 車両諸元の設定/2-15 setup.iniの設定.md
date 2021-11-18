# **2-15 setup.iniの設定**   
# やること
アセットコルサでは、`C:\Program Files (x86)\Steam\steamapps\common\assettocorsa\content\cars\○○\date`にある`setup.ini`でピット画面でのセットアップ調整の項目や幅を設定しています。


# ファイルの構成
### setup.iniファイルの構成
`[WING_]`  
  +　ウイングのセットアップ設定。  
 
`[PRESSURE_]`  
  +　タイヤ空気圧のセットアップ設定。  

`[CAMBER_]`  
  +　キャンバーのセットアップ設定。  

`[TOE_OUT_]`  
  +　トーのセットアップ設定。  

`[DAMP_BUMP_]`  
  +　ダンパーのセットアップ設定。  

`[DAMP_FAST_BUMP_]`  
  +　ダンパーのセットアップ設定。  

`[DAMP_REBOUND_]`  
  +　ダンパーのセットアップ設定。  

`[DAMP_FAST_REBOUND_]`  
  +　ダンパーのセットアップ設定。  


`[SPRING_RATE_]`  
  +　スプリングのセットアップ設定。  

`[ROD_LENGTH_]`  
  +　ロッド長のセットアップ設定。  

`[ARB_]`  
  +　アンチロールバーのセットアップ設定。 


`[FRONT_BIAS]`  
  +　ブレーキバランスのセットアップ設定。 

 

# 作業内容
### 全般の設定
1. `C:\Program Files (x86)\Steam\steamapps\common\assettocorsa\content\cars\○○\date`にある`setup.ini`を開く　　
2. ピットでセットアップを変更したい場合、その調整幅をここで設定する。何もしない場合ばいままで設定していたパラメータが適用されているのでピットで調整したい場合のみ入力する。
3. `SHOW_CLICKS=`で衝突範囲の3Dボックスのサイズを指定。単位は[m]。
4. `TAB=`にセットアップで表示するタブの名称を記入する。デフォルトのタブと整合性がとれるようにAERO,TYRES,SUSPENSION,ALIGNMENT,DAMPERS,DRIVETRAIN,GENERICのいずれかを使用しないとクラッシュするので注意。  
5. `MIN=`でセットアップ変更できる最小値を指定。単位は各項目によって異なる。
6. `MAX=`でセットアップ変更できる最大値を指定。  
7. `STEP=`で調整の段階幅を指定。
8. `POS_X=`でX軸の位置を指定。0：左、0.5：中央、1：右
9. `POS_Y=`でY軸の位置を指定。0から8の範囲。  
10.`HELP=`でマウスカーソルを合わせたときに表示される注釈の内容を指定。


以上で[2-15 setup.iniの設定](https://github.com/JSAE-ARCHIVES/MOD-Tutorial/blob/main/2%E7%AB%A0%20%E8%BB%8A%E4%B8%A1%E8%AB%B8%E5%85%83%E3%81%AE%E8%A8%AD%E5%AE%9A/2-08%20%E3%82%A8%E3%83%B3%E3%82%B8%E3%83%B3%E3%81%AE%E8%A8%AD%E5%AE%9A.md)は終了です。  
お疲れ様でした。  

| Back | Next |
|:---:|:---:|
| [2-014 エンジンの設定](https://github.com/JSAE-ARCHIVES/MOD-Tutorial/blob/main/2%E7%AB%A0%20%E8%BB%8A%E4%B8%A1%E8%AB%B8%E5%85%83%E3%81%AE%E8%A8%AD%E5%AE%9A/2-08%20%E3%82%A8%E3%83%B3%E3%82%B8%E3%83%B3%E3%81%AE%E8%A8%AD%E5%AE%9A.md) | [2-12 サスペンションの設定](https://github.com/JSAE-ARCHIVES/MOD-Tutorial/blob/main/2%E7%AB%A0%20%E8%BB%8A%E4%B8%A1%E8%AB%B8%E5%85%83%E3%81%AE%E8%A8%AD%E5%AE%9A/2-09%20%E3%82%B5%E3%82%B9%E3%83%9A%E3%83%B3%E3%82%B7%E3%83%A7%E3%83%B3%E3%81%AE%E8%A8%AD%E5%AE%9A.md) |
