# 形象版＋可維護版最終版｜部署與維護說明

## 資料夾內容
- `index.html`：網站主頁
- `site-config.json`：網站標題、人物文字、KPI、附件連結、AI 工具網址
- `ledger-data.csv`：台帳月份資料，可用 Excel 直接維護
- `assets/logo.png`：公司 Logo
- `assets/portrait.jpg`：形象照
- `assets/ip.jpg`：個人 IP 視覺圖

## 你平常只要改這兩個檔案
### 1. 改網站文字與按鈕
打開 `site-config.json`
- siteTitle：網站標題
- siteSubtitle：副標
- heroBadge：首頁小標籤
- managerQuote：主管一句話版本
- ownerName / ownerRole / ownerIntro：人物介紹
- kpis：KPI 數字
- attachmentLinks：附件 A-D 連結
- aiToolName / aiToolUrl：AI 工具按鈕

### 2. 改圖表資料
用 Excel 打開 `ledger-data.csv`
- month：月份
- total：總採購金額
- green：綠色採購金額

存檔後重新部署，圖表就會更新。

## 上傳到 Vercel
1. 到 Vercel 建立新專案
2. 上傳整個資料夾 `green_procurement_final_brand_maintainable`
3. 確認以下檔案都在同一個專案裡：
   - index.html
   - site-config.json
   - ledger-data.csv
   - assets 資料夾
4. 部署後即可取得網址

## 建議維護流程
1. 先改 `ledger-data.csv`
2. 再改 `site-config.json`
3. 本機預覽確認
4. 重新部署

## 適合後續再擴充
- 增加更多 KPI 卡片
- 串接更多附件下載區
- 接入正式 AI 採購判斷工具
- 加入簡報下載或教育訓練教材入口
