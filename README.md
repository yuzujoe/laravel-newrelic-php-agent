# laravel-newrelic-php-agent
Laravel の Docker 環境で [New Relic PHP Agent](https://docs.newrelic.com/docs/apm/agents/php-agent/getting-started/introduction-new-relic-php/) を動かすためのサンプルリポジトリです。

## 環境構築

direnv で環境変数を読み込むため、`.envrc` ファイルを作成します。

```shell
cp .envrc.sample .envrc
```

`.envrc` ファイルを編集して `direnv allow` を実行します。

New Relic API Key は [New Relic のダッシュボード](https://docs.newrelic.com/docs/apis/intro-apis/new-relic-api-keys/) から取得してください。

```shell

docker compose で環境を構築します。

```shell
docker compose build
docker compose up 
```

http://localhost にアクセスして Laravel の画面が表示されれば成功です。

最後に New Relic の画面が表示されることを確認してください。

<img width="2036" alt="Screenshot 2024-05-12 at 23 29 17" src="https://github.com/yuzujoe/laravel-newrelic-php-agent/assets/39491874/5cba640a-f42b-4914-94e2-0b3febbc9e26">
