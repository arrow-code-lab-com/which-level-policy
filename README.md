# which-level-policy
駐車アプリのポリシー

## 公開

`main` に push すると GitHub Actions（`.github/workflows/deploy.yml`）が GitHub Pages へ公開します。

- プライバシーポリシー: https://which-level.arrow-code-lab.com/
- 利用規約: https://which-level.arrow-code-lab.com/terms.html
- 特定商取引法に基づく表記: https://which-level.arrow-code-lab.com/legal.html
- アプリを入れる（端末に合うストアへ振り分け）: https://which-level.arrow-code-lab.com/app.html
  - アプリの共有文がこの URL を載せて送り先へ渡るので、ファイル名は変えないでください
  - App Store で公開したら、`app.html` の `APP_STORE_ID` にアプリ ID を入れてください。それまで iPhone では「準備中」と出ます

カスタムドメインは `which-level.arrow-code-lab.com` です。DNS に `which-level` → `arrow-code-lab-com.github.io` の CNAME レコードが必要です。
