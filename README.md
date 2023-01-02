# mypkg
[![test](https://github.com/Yoshino0304/mypkg/actions/workflows/test.yml/badge.svg)](https://github.com/Yoshino0304/mypkg/actions/workflows/test.yml)

talker.pyで送った数字のカウントをlistener.pyで表示するプログラムです.

# 動作手順
1. GithubのサイトでcodeからHTTPSへ移動し, URLをコピーする.
1. ```$ git clone https://github.com/Yoshino0304/mypkg.git```
1. 実行する.

* 実行例

```
$ cd mypkg
```
ここから2つのパターンに分かれる. 

* パターン1: 1つの端末で実行.

2つのノードをトピックで連結し, ノード間でやり取りをする方法

```$ ros2 launch mypkg talk_listen.launch.py```

talk_listen.launch.pyを使用することによってtalkerとlistenerの2つのノードを1度に立ち上げている. 

* パターン2: ２つの端末で実行.

1つ目の端末での操作

```$ ros2 run mypkg talker```

talkerノードの実行をしている.

2つ目の端末での操作

```$ ros2 run mypkg listener```

listenerノードの実行をしている.

これでtalker.pyが送った数字をlistener.pyで表示できる.
# 必要なソフトウェア
* Python 3.10.6
* ROSのバージョン　ROS2

# 動作確認済み環境
* Ubuntu 22.04.1LST

# ライセンス
* このソフトウェアパッケージは，3条項BSDライセンスの下，再頒布および使用が許可されます．
* © 2022 Taiki Yoshino
