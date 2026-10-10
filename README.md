# 脊椎スコアブック

脊椎の評価・分類・計測スコア22項目を、入力と同時に計算するWebアプリです。
結果は「カルテ用にコピー」で電子カルテに貼り付けられるテキストになります。
入力内容は端末内だけで計算され、このサイト（GitHub）には送信されません。

公開URL：https://spinesurgueda-droid.github.io/spine_clinical_scores/

## 収録スコア

| 分野 | スコア |
|---|---|
| 頚椎・頚髄症 | JOAスコア（17点）、mJOA（18点）、Nurick 分類、NDI |
| 腰椎 | JOAスコア（29点）、ODI |
| 外傷・脊髄損傷 | ASIA Impairment Scale、TLICS、SLIC |
| 脊椎腫瘍 | SINS、改訂徳橋スコア、富田スコア、Bilsky 分類、McCormick 分類 |
| 脊柱アライメント | SRS-Schwab 分類、GAP スコア |
| 計測・改善率 | 改善率（平林法）、Meyerding 分類、Genant 半定量法、OPLL 占拠率 |

## ファイル構成

| ファイル | 役割 |
|---|---|
| index.html | アプリ本体 |
| manifest.webmanifest | ホーム画面に追加したときの名前・アイコンの設定 |
| sw.js | オフラインでも起動できるようにする仕組み |
| icon-180.png / icon-192.png / icon-512.png | ホーム画面のアイコン |

## iPhoneに入れる

Safari で https://spinesurgueda-droid.github.io/spine_clinical_scores/ を開く →「共有」→「ホーム画面に追加」→「追加」

## アプリを更新するとき

1. 新しい `index.html` を受け取る
2. GitHub のリポジトリ画面で「Add file」→「Upload files」→ 新しい `index.html` をアップロード →「Commit changes」
3. 1〜3分後にアプリを開き直すと新しい版になります（反映されないときはアプリを完全に閉じて再起動）

## 注意

- 臨床判断の補助を目的とした計算ツールです。各スコアの判定基準は原著・各学会の最新版で確認してください。
- ODI・NDI・mJOA の設問文は原版の趣旨に沿って日本語で要約したもので、公式日本語版とは文言が異なります。研究・正式な記録には公式版の質問票を使用してください。
