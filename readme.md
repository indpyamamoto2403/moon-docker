プロジェクトセットアップ手順
このプロジェクトでは、WSLとDockerを使用してフロントエンドとバックエンドをセットアップし、MySQLデータベースにアクセスします。以下の手順に従って開発環境を構築してください。

1. WSLへの接続
まず、WSL（Windows Subsystem for Linux）に接続してください。以下のコマンドをPowerShellまたはコマンドプロンプトで実行します。

bash
コードをコピーする
wsl
2. Dockerイメージの取得
次に、Dockerを使用して moon-docker イメージをプルします。以下のコマンドを実行して、イメージを取得してください。

bash
コードをコピーする
docker pull moon-docker
3. フロントエンドおよびバックエンドの作成
プロジェクトのルートディレクトリに移動し、それぞれのフォルダを作成します。

bash
コードをコピーする
mkdir front-end
mkdir back-end
4. Gitリポジトリからソースコードを取得
各フォルダ内で、Gitリポジトリから最新のソースコードをプルします。

フロントエンド
bash
コードをコピーする
cd front-end
git pull origin main
バックエンド
bash
コードをコピーする
cd back-end
git pull origin main
5. 開発作業について
フロントエンド の開発は、front-end ディレクトリ内で行います。
バックエンド の開発は、back-end ディレクトリ内で行います。
6. MySQLへのアクセス
MySQLへのアクセスには、mysql コマンドが使えないため、MySQL Workbench を使用してデータベースに接続します。以下の情報を使って接続設定を行ってください。

ホスト名: localhost
ポート: 3306
ユーザー名: root
パスワード: your_password
