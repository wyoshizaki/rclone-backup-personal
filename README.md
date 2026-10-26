# rclone-backup-personal — public information site

個人用rcloneバックアップ構成の説明と、プライバシーポリシーを掲載する静的サイトです。
このリポジトリはバックアッププログラムやバックアップデータの保存先ではありません。

## ページ

- `index.html` — アプリの説明・要求権限・連絡先
- `privacy.html` — アクセス、利用、保存、提供、削除の方針
- `assets/tokens.css` — V-Sidoを参考にした配色トークン
- `assets/site.css` — レイアウトとレスポンシブ表示
- `.nojekyll` — 静的ファイルをそのまま公開する指定

HTMLとCSSのみ。ビルド、JavaScript、npm、外部フォント、解析サービス、フォームは不要です。
`index.html`をブラウザーで開けばローカルでも表示できます。

## GitHub Pagesの公開設定（まだ実施前の手順）

1. 公開リポジトリ `wyoshizaki/rclone-backup-personal` を用意します。
2. このサイトのファイルだけを`main`ブランチ直下へ配置します。
3. Settings → Pages → Deploy from a branch → `main` / `(root)`を選んで保存します。
4. 実際のPages URLで、ホームとプライバシーポリシーの両方を未ログインで確認します。

予定URL（公開・到達確認前にはGoogle設定に入力しない）：
- ホーム：`https://wyoshizaki.github.io/rclone-backup-personal/`
- プライバシー：`https://wyoshizaki.github.io/rclone-backup-personal/privacy.html`

サイトを公開することと、Googleでのドメイン受理、所有確認、OAuthの本番化、審査は別です。
承認済みドメインにはURLやパスではなく、Googleが求める登録可能ドメインを使用します。
`wyoshizaki.github.io`の受理や必要な所有確認は、実際のGoogle管理画面で別途確認してください。
`github.io`全体を自分の所有ドメインとして申告しないでください。
Search Consoleによる所有確認を求められた場合は、同じGoogleアカウントでURLプレフィックス方式等の対応を確認します。
架空の確認ファイル・メタタグは事前に用意しません。

## 公開してはいけないもの

Drive・Photosの実データ、Takeout ZIP、rclone.conf、OAuthトークン、クライアントシークレット、
暗号化鍵、作業ログ、本人用の機器・アカウント記録、画面写真をコミットしないでください。
`.gitignore`だけで機密情報の混入を防げるわけではありません。公開前にファイル一覧を確認します。

## デザイン

運用者指定の `wyoshizaki/vsido-design` を参照しています。
白いパネル、青いヘッダー、少量の黄色、CSS変数による配色、十分なコントラストを採用。
個人用アプリであることを明確にするため、企業のロゴは転載せず、アプリ名をヘッダーに表示します。
詳細と参照コミットは `DESIGN_NOTES.md` を参照してください。

## 運用上の注意

これは個人用アプリの設計とデータ取り扱いを説明するサイトです。
公開によってバックアップが動き始めたり、Googleに承認されたりするものではありません。
外部監視等の追加や実装変更時は、プライバシーポリシーとの整合性を確認してください。
鍵・認証情報のない状態でWebサイトをテストします。
