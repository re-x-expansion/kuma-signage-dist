# kuma-signage-dist

球磨村 施設予約サイネージの端末へ配る、署名付きの配布物（Releases）だけを置く公開リポジトリです。ソースコードは置いていません。

- 端末（ラズパイ）が、毎晩 `releases/latest/download` から `VERSION`・`bundle.tar.gz`・`bundle.tar.gz.sig` を取得し、**署名を検証してから**適用します。
- 配布物は本体リポジトリ（非公開）の GitHub Actions が作成・署名して公開します。**手作業でファイルを置かないでください**（署名が合わない配布物は端末が受け付けません）。
- 配布物に、個人情報・パスワード・CSV の URL は含まれません。
