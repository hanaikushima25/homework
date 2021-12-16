# ロボットシステム学2021年度課題１
2021年度ロボットシステム学の課題1で作成したデバイスドライバです。

## インストール＆アンインストール
### インストール
```
$ git clone git@github.com:hanaikushima25/myled.git
$ cd myled
$ make
$ sudo insmod myled.ko
$ sudo chmod 666 /dev/myled0
```
### アンインストール
```
$ sudo rmmod myled
```
## LEDの点灯、消灯
### LED点灯
```
$ echo 1 > /dev/myled0
```
### LED消灯
$ echo 0 > /dev/myled0
