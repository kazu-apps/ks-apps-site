# App Store リスティング用の画像(配信専用)

`03_開発/ks-receipt/docs/assets/listing/` の生成物を、App Store リスティングへ
アップロードするために公開配信しているコピー。

Shopify のリスティング編集フォームにはローカルファイルを直接渡せないため
(claude-in-chrome の file_upload は「ユーザーが共有したファイル」しか受け付けず、
ローカルサーバーへの fetch は Chrome の Private Network Access で遮断される)、
GitHub Pages の CORS 許可(`Access-Control-Allow-Origin: *`)を使って
ページ内 fetch → File 化 → input 注入する経路に載せている。

**原本はアプリ側リポジトリ**。ここは手で編集せず、`npm run listing:all` で
再生成したものをコピーすること。
