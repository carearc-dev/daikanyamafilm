DAIKANYAMA FILM — GitHub Pages 公開ファイル

このフォルダの中身をGitHubリポジトリの公開ルートにアップロードしてください。
index.html / 404.html / assets / img が公開用ファイルです。

重要:
このビルドは独自ドメインなど、URLのルート (https://example.com/) に公開する設定です。
GitHub Pagesの標準URL https://ユーザー名.github.io/リポジトリ名/ にそのまま置く場合、
assets・画像・ページ内リンクがリポジトリ名以下を向くよう再ビルドが必要です。
既存ドメインを使う場合は、GitHubリポジトリ Settings > Pages > Custom domain にドメインを設定し、
ドメイン管理会社側でGitHub PagesのDNS設定を行ってください。

直接アクセス時の /works /cast /news /lp は404.htmlからSPAを起動します。
問い合わせフォームの送信先は未設定です。送信を有効化するには、ソースをビルドする際に
VITE_FORMSPREE_IDを設定してください（手順は同梱ZIPのプロジェクトREADMEを参照）。
