# 85mm 静的ホームページ

2026年10月27日に確認した https://85mm.blog/ の「リニューアルちゅう」画面をHTML・CSSで再現しました。

- `index.html` をブラウザで開くと表示できます。ビルド・外部サービスは不要です。日時表示のためにJavaScriptを使用します。
- `styles.css` で色、余白、文字サイズ、傾きを変更できます。
- 日付・時刻は日本時間（Asia/Tokyo）を表示します。ページを開いた直後、1秒ごと、およびタブに戻った際に更新します。表示は分単位です。閲覧端末の時計を使用します。
- 書体 Darumadrop One を同梱しています。ライセンスは `OFL.txt` を参照してください。
- ブログ記事一覧などの下層ページは含みません。

## GitHub Pagesでの公開

1. 公開先リポジトリのルートに `index.html`、`styles.css`、`darumadrop-one.ttf`、`OFL.txt`、`.nojekyll` を配置します。`85mm-static/` フォルダ自体をルートの下に入れないでください。
2. GitHubの Settings → Pages → Build and deployment で、Source を Deploy from a branch、Branch を main / (root) にして保存します。
3. GitHub Pagesの公開完了後、発行されたURLで表示を確認します。
4. 独自ドメインは Pages → Custom domain に設定した後、DNS管理サービスでGitHub Pages用のレコードを設定します。設定値は接続するドメインとアカウントに合わせて確認してください。
5. DNSの検証と証明書発行後に Enforce HTTPS を有効にします。

公開先: https://github.com/yg0402/85mm-static
独自ドメイン: https://85mm.blog/
公開方式: main ブランチ / (root)。
公式手順: https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site
