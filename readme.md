# プロジェクトセットアップ手順
このプロジェクトでは、WSL（Windows Subsystem for Linux）とDockerを使用してフロントエンドとバックエンドをセットアップし、MySQLデータベースにアクセスします。以下の手順に従って開発環境をセットアップしてください。

## 1. WSLに接続する
まず、WSL（Windows Subsystem for Linux）に接続します。PowerShellまたはコマンドプロンプトで次のコマンドを実行します。
```bash
wsl
```

## 2. Dockerイメージを取得する
次に、Dockerを使用してmoon-dockerイメージを取得します。以下のコマンドを実行してイメージを取得します。
```dockerfile
docker pull moon-docker
```

## 3. フロントエンドとバックエンドを作成する
プロジェクトのルートディレクトリに移動し、それぞれのフォルダを作成します。

## 4. Gitリポジトリからソースコードを取得する
各フォルダ内で、Gitリポジトリから最新のソースコードを取得します。

```bash
cd front-end
git pull origin main
```

```bash
cd back-end
git pull origin main
```

## 5. 開発のワークフロー
フロントエンドの開発はfront-endディレクトリで行います。
バックエンドの開発はback-endディレクトリで行います。

## 6. MySQLにアクセスする
MySQLにアクセスするには、mysqlコマンドを使用することはできません。代わりにMySQL Workbenchを使用してデータベースに接続します。以下の情報を使用して接続を設定します。

ホスト：localhost
ポート：3308(コンテナ側は3306)
ユーザー名：root
パスワード：your_password


