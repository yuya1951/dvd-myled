# myled
ロボットシステム学2020　課題1用


# テーマ
ラズベリーパイ4B+において、デバイスドライバを用い、ledを点灯させる。

[youtube動画](https://www.youtube.com/watch?v=uexH9YN6MUI&feature=youtu.be)

# 内容
３つのledを用い、いろいろな組み合わせで点滅させる。

# 使用方法
0．GPIO23、24、25　にそれぞれLEDの+側につなぎ、GNDを-側につなぐ。

1．まず、以下のコマンドでこのリポジトリをクローンする。

    $git clone https://github.com/yuya1951/dvd-myled.git
    
2．makeする

    $make
    
3．モジュールをインストールする。

    $sudo insmod myled.ko
    
4．出来上がった/dev/myled0のパーミッションを変更する。

    $sudo chmod 666 /dev/myled0
   
5．すべてのLEDを消す。

    $echo 0 > /dev/myled0
   
6．最初は、1つずつ点く。その後、２つ、3つとなり、最後に全部消える。

    $echo 2 > /dev/myled0
    
7．チカチカする。同じ動きを3周する。

    $echo 3 > /dev/myled0
    
 
# 参考にしたもの
[千葉工業大学　上田先生の作成したリポジトリ](https://github.com/ryuichiueda/robosys_device_drivers)

# ライセンス
[ライセンス](https://github.com/yuya1951/dvd-myled/blob/main/COPYING)

[Lisense](https://github.com/yuya1951/dvd-myled/blob/main/COPYING)


#supporter
[tanapol](https://github.com/TanapolHongsuwan/LED-RaspPi-DeviceDrivers)
