# mypkg
[![test](https://github.com/Yoshino0304/mypkg/actions/workflows/test.yml/badge.svg)](https://github.com/Yoshino0304/mypkg/actions/workflows/test.yml)

talker.pyで送った数字のカウントをlistener.pyで表示するプログラムです.

# 動作手順
1. GithubのサイトでcodeからHTTPSへ移動し, URLをコピーする.
1. ```$ git clone https://github.com/Yoshino0304/mypkg.git```
1. 実行する.

* 実行例

````
$ cd mypkg
$ colcon build
````
* パターン1:1つの端末で実行.

```$ ros2 launch mypkg talk_listen.launch.py```

talk_listen.launch.pyを使用することによってtalkerとlistenerの2つのノードを1度に立ち上げている. 

* パターン2:２つの端末で実行.

1つ目の端末での操作

```$ ros2 run mypkg talker```talkerノードの実行

2つ目の端末での操作

```$ ros2 run mypkg listener```listenerノードの実行

これでtalker.pyが送った数字をlistener.pyで表示できる.
# 必要なソフトウェア
* Python 3.7～3.10
* ROSのバージョン　ROS2

# 動作確認済み環境
* Ubuntu 22.04.1LST

# ライセンス
* このソフトウェアパッケージは，3条項BSDライセンスの下，再頒布および使用が許可されます．
* © 2022 Taiki Yoshino
