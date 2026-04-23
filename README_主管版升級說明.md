# 主管版升級包｜使用說明

## 這次已完成的 1+2+3
1. 已改成主管版 HTML
2. KPI 改為「綠色採購品項占比」，資料來源為 `item-share-data.csv`
3. 已加入紅黃綠燈版狀態判讀

## 你指定的修改都已完成
- 已刪除「形象整合 / 制度網站也保有你的個人 IP 風格」區塊
- 「主管一句話版本」已改為「核心重點」
- KPI 已改為綠色採購品項占比
- 已刪除底部內部說明文字
- 名字已改為「GADM-BO 曉君」

## 怎麼維護
### A. 改網站文字
修改 `site-config.json`

### B. 改品項占比
用 Excel 打開 `item-share-data.csv`
欄位說明：
- category：品項類別
- amount：金額
- note：備註

修改後存檔、推送 GitHub，Vercel 會自動更新。

## 建議下一步
把正式附件網址與 AI 工具網址補到 `site-config.json`。
