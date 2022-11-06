# Docker Playgorund - ruby

コンテナ上でrubyの実行環境を構築しVisual Studio Codeから接続・実行できる環境を提供する

コンテナイメージのベースは
[ruby:slim-bullseye](https://hub.docker.com/_/ruby)
を利用。最新の最小限の環境としている。

追加で以下をインストールしている

* `git`
* `curl`
* `gcc`
* `make`

実行ユーザ:`vscode`  
ワークスペース:`/opt`  

ホスト側の`opt`フォルダをコンテナ側の`/opt`としてマウントしている

gemで以下をインストール済み

* rubocop
* rails
* rails-api

以下のVisual Studio Code 拡張をインストール

* rebornix.Ruby

## 使い方

[Docker Desktop](https://www.docker.com/products/docker-desktop/)を立ち上げる

[Visual Studio Code](https://azure.microsoft.com/ja-jp/products/visual-studio-code/)に[Dev Containers](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers)をインストール

後は Dev Containerで起動する
