# 宿泊客集計 PWA

## 公開方法（GitHub Pagesの例）
1. GitHubで新しい公開リポジトリを作成します。
2. このZIPを解凍し、中の `index.html` `manifest.json` `sw.js` `icon-192.png` `icon-512.png` をリポジトリ直下へアップロードします。
3. GitHubのリポジトリで Settings → Pages を開き、Deploy from a branch、`main`、`/(root)` を選択して保存します。
4. 数分後に表示される `https://ユーザー名.github.io/リポジトリ名/` をAndroidのChromeで開きます。
5. Chrome右上の︙メニューから「アプリをインストール」または「ホーム画面に追加」を選びます。

## データについて
このPWAは `localStorage` の `hotelNationalityRecordsV1` を使います。アプリ内のデータは同じブラウザ・同じサイト内で保存されます。
ChatGPT内のアプリと公開サイトは保存領域が別なので、ChatGPT内アプリにあるデータを移す場合は、ChatGPT内アプリからJSONバックアップを出し、このPWAでJSON復元してください。
ブラウザのデータ削除や端末変更に備えて、定期的にJSONバックアップを保存してください。

## 注意
GitHub PagesなどHTTPSで公開されたURLが必要です。ZIPをスマホに保存しただけではホーム画面アプリとしてインストールできません。
