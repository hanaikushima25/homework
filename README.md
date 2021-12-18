# ロボットシステム学2021年度課題１
2021年度ロボットシステム学の課題1で作成したデバイスドライバです。
## 環境
  - Raspberry Pi 4 Computer Model B
  - OS:ubuntu 18.04 LTS
## 実行
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
```
$ echo 0 > /dev/myled0
```
## 実行結果
  Youtube: https://www.youtube.com/watch?v=_Pf2KzTTuEA
## 文責
 - Hana Ikushima
 - s20C1006NU@s.chibakoudai.jp
## 参考
 - Minori Katou
   https://github.com/MinoriKatou/LED
 - https://tips-memo.com/python-readme
## ライセンス
　"myled" is under GNU General Public License v2.0.
 
 Thank you!
