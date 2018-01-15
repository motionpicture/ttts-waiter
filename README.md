# TTTS-WAITER

[![CircleCI](https://circleci.com/gh/motionpicture/ttts-waiter.svg?style=svg&circle-token=5ab628a88db4f2535912addc2e77a0aad3b6f04e)](https://circleci.com/gh/motionpicture/ttts-waiter)

## Table of contents

* [Background](#background)
* [Usage](#usage)
* [Jsdoc](#jsdoc)
* [License](#license)

## Background
see [waiter repository](https://github.com/motionpicture/waiter)

## Usage

### インフラ
#### web server
node.js application  
- nginx on [GCP AppEngine](https://cloud.google.com/appengine/?hl=ja)

#### DB
- Redis Cache

### Environment variables

| Name                     | Required | Value    | Purpose                                   |
| ------------------------ | -------- | -------- | ----------------------------------------- |
| `DEBUG`                  | false    | waiter:* | Debug                                     |
| `NODE_ENV`               | true     |          | 許可証暗号化の秘密鍵                       |
| `WAITER_PASSPORT_ISSUER` | true     |          | 許可証発行者識別子(通常発行APIのドメインを指定) |
| `WAITER_RULES`           | true     |          | 発行規則リスト                               |
| `WAITER_SECRET`          | true     |          | 許可証暗号化の秘密鍵                       |
| `REDIS_HOST`             | true     |          | Redis Cache接続ホスト                        |
| `REDIS_PORT`             | true     |          | Redis Cache接続ポート                        |
| `REDIS_KEY`              | true     |          | Redis Cache接続キー                         |

## Jsdoc

`npm run doc`でjsdocを作成できます。./docに出力されます。

## License

UNLICNSED
