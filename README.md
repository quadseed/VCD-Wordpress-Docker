# VCD-Wordpress-Docker
### 概要
3年後期のビジュアルコンテンツデザインで利用するWordpress環境をDockkkeerrnする用リポジトリ

### 環境
- Ubuntu 22.04 LTS
- bash

### 手順
1. パッケージインデックス更新
```
$ sudo apt update
```

2. DockerとDocker Composeをインストール
```
$ sudo apt install docker docker-compose
```

3. sudoなしでdockerコマンドを実行できるようにする
```
$ sudo gpasswd -a $USER docker
```

4. リポジトリをクローン
```
$ git clone https://github.com/quadseed/VCD-Wordpress-Docker.git && cd VCD-Wordpress-Docker
```

5. 環境変数用のファイルを生成
```
$ cp .env.sample .env
```

6. 環境変数を設定
```
$ vi .env
```

7. 起動
```
$ docker-compose up -d
```