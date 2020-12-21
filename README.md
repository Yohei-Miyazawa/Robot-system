# Robot-system
千葉工業大学　未来ロボティクス学科４S

ロボットシステム学　課題１

# 概要
LEDを点灯させるデバイスドライバを作成した

上田准教授が講義で作成したコードのライセンスを整備したものである

上田准教授のデバイスドライバ作成動画：https://youtu.be/xQW8-FNuboo　　

# 環境
・ハード Raspberry Pi4 ModelB

・ソフト Ubuntu18.04

# 使用した道具
・LED（緑）

・抵抗(220Ω)

・ブレッドボード

・ジャンパ線

# 回路
GPIO25（22番ピン）とGND（39番ピン）の間にLEDを接続

・LEDのアノードをGPIO25に繋ぐ

・LEDとGNDの間に抵抗を繋ぐ

# デモ
デモ動画：https://youtu.be/PtjcwzEXh-Q

# インストール方法
```
$ git clone https://github.com/Yohei-Miyazawa/Robot_system.git
$ cd Robot_system/
$ make
$ sudo insmod myled.ko
$ sudo chmod 666 /dev/myled0
```

#　実行方法
```
$ echo 1 > /dev/myled0
$ echo 0 > /dev/myled0
```
LEDはecho 1を入力した際に点灯し、echo 0を入力すると消灯する

# ライセンス

このリポジトリはGPLv3が付与されている

