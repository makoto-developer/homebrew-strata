# homebrew-strata

[Strata](https://github.com/makoto-developer/strata) の Homebrew tap です。

Strata は、マイクロサービスのコードを「層」として読むための依存関係・コールグラフ可視化ツールです。
gRPC・REST・GraphQL をまたいで、関数レベルで処理を追えます。

## インストール

```sh
brew tap makoto-developer/strata
brew trust makoto-developer/strata   # 公式以外の tap は明示的な信頼が必要(Homebrew の仕様)
brew install strata

strata --version
strata serve ./my-monorepo
```

`brew trust` を省くと `Refusing to load formula from untrusted tap` で止まります。
新しめの Homebrew が、公式以外の tap を既定では読み込まなくなったためです。

- **Apple Silicon (macOS 13 以降)**: Node.js を同梱した単一実行ファイルを配布します(Node のインストール不要)
- **Intel Mac / Linux**: ソースを配置し、Homebrew の `node` で実行します

## リンク

- 本体リポジトリ: https://github.com/makoto-developer/strata
- ドキュメント: https://makoto-developer.github.io/strata/
- 質問・不具合: https://github.com/makoto-developer/strata/issues

## ライセンス

Strata 本体は AGPL-3.0-only です。この tap(formula)は MIT とします。
