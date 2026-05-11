# azumacco.github.io

提案書・整理HTMLなどの共有用GitHub Pages。

## 公開URL

https://azumacco.github.io/

## 検索除外の方針

- `robots.txt` で全クローラー拒否
- 各HTMLの `<head>` に `<meta name="robots" content="noindex, nofollow">` を入れる
- リポジトリはPublicなのでコード自体は検索可能。**金額・固有名詞など機密度の高い内容は置かない**

## 運用ルール

- 配置場所: `<カテゴリ>/<案件名>.html`
  - 例: `proposals/client-a.html` → `https://azumacco.github.io/proposals/client-a.html`
- URL推測されたくない案件はパスをランダム化（例: `proposals/a1b2c3/index.html`）
- 更新後、反映まで1〜2分のタイムラグあり

## デプロイ

```bash
cd ~/Workspace/azumacco.github.io
# HTMLを配置
git add . && git commit -m "add: 案件名" && git push
```
