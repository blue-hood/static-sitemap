# static-sitemap

静的 Web サイトの sitemap.xml を生成します。

## 使い方

`$ sitemap (ドキュメントルート) (前バージョンのドキュメントルート) (html ファイル)...`

(例) 現在の Web サイトのドキュメントルートを html/、１つ前のバージョンのドキュメントルートを old/ とします。
html/ ディレクトリ下に index.html, articles/section.html, 404.html があるとき、
index.html と articles/section.html を含む sitemap.xml を作成する場合は

`$ sitemap html/ old/ index.html articles/section.html`

とします。

## changefreq と lastmod の生成アルゴリズム

html/ と old/ ディレクトリ内の html ファイルどうしを比較することで、changefreq と lastmod を生成します。
[詳しく](https://apps.bluehood.net/articles/sitemap/)
