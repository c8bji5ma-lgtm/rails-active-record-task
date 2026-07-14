# Rails Active Record Task

Active Recordの`joins`や`left_outer_joins`を使い、料理、店舗、住所、顧客の関連データを取得する課題用Railsアプリケーションです。

## 動作環境

- Ruby 4.0.5
- Ruby on Rails 8.1.3
- Bundler 4.0.10
- PostgreSQL 18.4
- Node.js 24.18.0
- Yarn 1.x

## セットアップ

PostgreSQLを起動した後、次のコマンドを実行してください。

```bash
bundle install
yarn install --frozen-lockfile
bundle exec rails db:prepare
```

ローカルのPostgreSQL設定が`config/database.yml`と異なる場合は、`DATABASE_URL`を指定できます。

```bash
DATABASE_URL=postgresql://user:password@localhost/delivery_launch_development \
  bundle exec rails db:prepare
```

## 起動

```bash
bundle exec rails server
```

## テスト

```bash
bundle exec rspec
```

## 環境変数

- `DATABASE_URL`: PostgreSQLへの接続URL（任意）
- `DELIVERY_LAUNCH_DATABASE_PASSWORD`: production用DBユーザーのパスワード
- `SECRET_KEY_BASE`: production環境のsecret key base
