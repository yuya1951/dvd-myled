# myled
ロボットシステム学2020　課題1用

# テーマ
ラズベリーパイ4B+において、デバイスドライバを用い、ledを点灯させる。

# 内容
３つのledを用い、いろいろな組み合わせで点滅させる。

# 使用方法
1．まず、以下のコマンドでこのリポジトリをクローンする。
    $git clone https://github.com/yuya1951/dvd-myled.git
    
2. makeする
    $make
    
3. モジュールをインストールする。
    $sudo insmod myled.ko
    
4. 出来上がった/dev/myled0のパーミッションを変更する。
    $sudo chmod 666 /dev/myled0
    
5．
    $echo 2 > /dev/myled0
    
6．
    $echo 3 > /dev/myled0
    
 
# 参考にしたもの
[千葉工業大学　上田先生の作成したリポジトリ](https://github.com/ryuichiueda/robosys_device_drivers)

# ライセンス
[ライセンス](https://github.com/yuya1951/dvd-myled/blob/main/COPYING)

[Lisense](https://github.com/yuya1951/dvd-myled/blob/main/COPYING)

