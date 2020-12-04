# Robot-system
千葉工業大学　未来ロボティクス学科４S

ロボットシステム学　課題１

# 概要
LEDを点灯させるデバイスドライバを作成した

上田教授が講義で作成したコードのライセンスを整備したものである

上田教授のデバイスドライバ作成動画：https://youtu.be/xQW8-FNuboo

# 使用した道具
・LED（緑）
・抵抗(220Ω)
・ブレッドボード
・ジャンパ線

# 実行方法
```
$ git clone https://github.com/ikeda-hitomi/robot_system.git
$ make
$ sudo insmod myled.ko
$ sudo chmod 666 /dev/myled0
```
```
$ echo 1 > /dev/myled0
$ echo 0 > /dev/myled0
```
LEDはecho 1を入力した際に点灯し、echo 0を入力すると消灯する

# デモ
デモ動画：https://youtu.be/PtjcwzEXh-Q

# 環境
・ハード Raspberry Pi4 ModelB
・ソフト Ubuntu18.04






