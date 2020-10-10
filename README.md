# dialog-system-with-cotoba-agent-oss

## 概要

2020年10月8日 18:00-20:00 に行われた「対話システム勉強会（第一回）OSSを利用した対話システムの作り方」の、「4. COTOBA Agent OSS による対話システムの実装」で使用したサンプルコードです。

https://cotobaagent-developers-community.connpass.com/event/188047/

- sample1: 一問一答型のサンプルコードを含むディレクトリ
- sample2: ネットワーク型のサンプルコードを含むディレクトリ
- sample3: AIML の変数の説明用のサンプルコードを含むディレクトリ
- sample4: スロットフィリング型のサンプルコードを含むディレクトリ
- sample5: 他の対話エンジンとの連携のサンプルコードを含むディレクトリ

## サンプルコードの動かし方

COTOBA Agent OSS (https://github.com/cotobadesign/cotoba-agent-oss) を
git clone で取得しセットアップを行った後、
cotoba-agent-oss/dialog-engine ディレクトリの直下に, 
sample1 〜 sample5 のディレクトリを配置してください。

```shell
$ cd cotoba-agent-oss/dialog-engine
$ ls -l
...
drwxr-xr-x  5 user  group   160 10  8 XX:XX sample1
drwxr-xr-x  5 user  group   160 10  8 XX:XX sample2
drwxr-xr-x  5 user  group   160 10  8 XX:XX sample3
drwxr-xr-x  5 user  group   160 10  8 XX:XX sample4
drwxr-xr-x  5 user  group   160 10  8 XX:XX sample5
...
```

上記のように sample1 〜 sample5 が表示されればOKです。
各サンプルコードを動かすには、下記を行って下さい。
（例）sample1 の場合
```shell
$ cd sample1/script
$ ./console.sh
```

## sample5 を動かすための雑談エンジンのセットアップ

sample5 は他の対話エンジンとの連携のサンプルコードとなっており、
OpenNMT で実装された雑談エンジンをセットアップして REST API サーバとして立ち上げておく必要があります。

https://github.com/junya-takayama/open2ch_chatbot_openNMT/

上記のリポジトリの README.md の手順に従って雑談対話システムの REST API を立ち上げた状態で、上記の sample5 サンプルコードを実行して下さい。
