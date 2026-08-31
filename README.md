# 存股資產追蹤（家人乾淨版）

跟你自己在用的那份完全一樣的程式（動態追蹤持股、Cloudflare 即時報價），
唯一差別：這份不含任何個人真實資料，家人打開後畫面是空白的，
會照著「尚未新增紀錄」的提示自行輸入自己的資料。

## 部署（跟原本一樣）

1. 開一個新的 GitHub repo（跟你自己那個分開，避免資料混在一起）
2. 放入這四個檔案：`index.html`、`manifest.webmanifest`、`_routes.json`、
   `functions/quote.js`（注意 quote.js 要放在 functions 資料夾裡）
3. Cloudflare Pages → Create → Pages → Connect to Git → 選這個新 repo
4. 部署完成後把網址分享給家人

## 資料隔離

每個人打開連結後，資料是依照各自登入的身分分開存放的，
不會共用同一份、也看不到彼此的資料，可以放心讓多個家人共用同一個網址。
