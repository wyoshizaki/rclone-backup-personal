# デザインと出典

## 指定された参照

- リポジトリ： https://github.com/wyoshizaki/vsido-design
- 参照コミット： `9719317dcbb70ca43b8acc1b1173556a730cdb21`
- 確認したファイル：
  - `plugins/vsido-design/skills/vsido-design/SKILL.md`
  - `plugins/vsido-design/skills/vsido-design/theme/at_theme.css`
  - `plugins/vsido-design/skills/vsido-design/theme/themes/brand.css`

白主体のパネルと青いヘッダー帯、色はCSS変数から参照する原則、
黄色を細い文字・線ではなく面として使う原則、コントラスト測定方針を参考にしています。
`assets/tokens.css`は参照先の役割・値に基づいてこのサイト用に書いたサブセットで、
参照先のCSS全文や共通JavaScriptを複製したものではありません。
参照元リポジトリは変更していません。

ロゴ画像は含めず、個人用アプリの名前をヘッダーに表示します。
この選択は、個人用アプリが会社提供の製品だと誤認されることを避けるためです。
フォントファイルは同梱しません。表示端末のシステムフォントを利用します。

## 仕様の確認先

- Google / OAuthブランドとポリシーの要件：
  https://developers.google.com/identity/verification/authentication-verification
- Google API Services User Data Policy：
  https://developers.google.com/terms/api-services-user-data-policy
- rclone / Google Drive・drive.readonly：
  https://rclone.org/drive/
- rclone / crypt：
  https://rclone.org/crypt/
- GitHub Pagesの公開手順：
  https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site
- GitHub PagesのIPアドレス記録：
  https://docs.github.com/en/pages/getting-started-with-github-pages/what-is-github-pages

参照元の権利・名称はそれぞれの権利者に帰属します。
Googleやrclone、V-Sidoの公式サービスとしての保証・審査承認を表示しません。
