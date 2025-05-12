# MkDocsへようこそ

完全なドキュメントは[mkdocs.org](https://www.mkdocs.org)をご覧ください。

## コマンド

* `mkdocs new [dir-name]` - 新しいプロジェクトを作成します。
* `mkdocs serve` - ライブリロード機能付きのドキュメントサーバーを起動します。
* `mkdocs build` - ドキュメントサイトをビルドします。
* `mkdocs -h` - ヘルプメッセージを表示して終了します。

## プロジェクトのレイアウト

    mkdocs.yml    # 設定ファイル
    docs/
        index.md  # ドキュメントのホームページ
        ...       # その他のマークダウンページ、画像、およびその他のファイル

## marmaid

``` mermaid
graph LR
  A[Start] --> B{Error?};
  B -->|Yes| C[Hmm...];
  C --> D[Debug];
  D --> B;
  B ---->|No| E[Yay!];
```