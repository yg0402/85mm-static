# 85mm 静的ホームページ

2026年10月27日に確認した https://85mm.blog/ の「リニューアルちゅう」画面をHTML・CSSで再現しました。

- `index.html` をブラウザで開くと表示できます。ビルド・JavaScript・外部サービスは不要です。
- `styles.css` で色、余白、文字サイズ、傾きを変更できます。
- 日付・時刻は固定です。`index.html` の表示テキスト、`datetime`、`aria-label` を編集してください。実際の現在時刻を自動表示するにはJavaScript等が必要です。
- 書体 Darumadrop One を同梱しています。ライセンスは `OFL.txt` を参照してください。
- ブログ記事一覧などの下層ページは含みません。

## GitHub Pagesでの公開

1. 公開先リポジトリのルートに `index.html`、`styles.css`、`darumadrop-one.ttf`、`OFL.txt`、`.nojekyll` を配置します。`85mm-static/` フォルダ自体をルートの下に入れないでください。
2. GitHubの Settings → Pages → Build and deployment で、Source を Deploy from a branch、Branch を main / (root) にして保存します。
3. GitHub Pagesの公開完了後、発行されたURLで表示を確認します。
4. 独自ドメインは Pages → Custom domain に設定した後、DNS管理サービスでGitHub Pages用のレコードを設定します。設定値は接続するドメインとアカウントに合わせて確認してください。
5. DNSの検証と証明書発行後に Enforce HTTPS を有効にします。

ドメインと公開先はまだ未設定です。
公式手順: https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site
