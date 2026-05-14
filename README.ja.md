# didbbs

認証にDID（Decentralized Identifiers）を使用する掲示板システム（BBS）です。

## デモ
- [DID BBS](https://didbbs.code4fukui.org)

## 機能
- DIDと電子署名を使用して、匿名でメッセージを投稿できます
- 投稿されたすべてのメッセージを一覧表示します

## 必要要件
- Denoランタイム環境

## 使い方
1. リポジトリをクローンします
2. Denoを使用してサーバーを起動します: `deno run --allow-net --allow-read --allow-write didbbs.js`
3. ブラウザで `http://localhost:8001` にアクセスし、Webアプリケーションを開きます

## データ / API
- BBSのデータは `bbs.json` という名前のJSONファイルに保存されます
- サーバーは以下の2つのAPIエンドポイントを提供します:
  - `/api/list`: すべてのBBSメッセージのリストを返します
  - `/api/add`: BBSに新しいメッセージを追加します（有効なDIDと電子署名が必要です）

## ライセンス
MIT License — 詳細は [LICENSE](LICENSE) を参照してください。
