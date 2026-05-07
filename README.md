# Kiwa Sales Designer

> 銷售頁分屏設計工具 — 給 Kiwa Agency 行銷與設計團隊使用

基於 Ryan Hung《行銷設計雙重輸出》課程的五大層級框架。三欄式設計：分屏列表/檢核 + 文案編輯 + 1080×1080 即時預覽。

**生產環境**：https://sales-tool.kiwa-tw.co

---

## 功能

- **5 大層級框架**：版頭 / 訴求 / 商品 / 信任 / 收單
- **6 種版面分割**：單一、左右、三重點、四分割、圓形、表格化
- **即時預覽**：1080×1080 等比 canvas，文字、字體、顏色即時更新
- **直向堆疊**：「全部展開」模式模擬真實銷售頁從上到下閱讀
- **雙擊編輯**：在預覽直接雙擊文字修改，左側編輯器同步更新
- **SOP Checklist**：17 項檢核點，確保產出品質
- **匯出**：JSON 草稿 / 列印 PDF
- **開發者模式**：Alt+D 顯示元件 `data-dev` 名稱，方便溝通修改

## 鍵盤快捷鍵

| 快捷鍵 | 功能 |
|--------|------|
| `Cmd ←` / `Cmd →` | 切換上一屏 / 下一屏 |
| `Alt + D` | 開關開發者模式 |
| `雙擊文字` | 進入編輯模式 |
| `Enter` | 編輯時儲存 |
| `Esc` | 編輯時取消 |
| `Shift + Enter` | 編輯時換行 |

---

## 部署

純靜態 HTML，無 build step。

**Cloudflare Pages**（建議）
1. 連結此 repo
2. Build command：（留空）
3. Build output directory：`/`
4. Custom domain：`sales-tool.kiwa-tw.co`

## 開發

直接編輯 `index.html`，本機用瀏覽器開啟測試。沒有任何依賴。

---

## 後續整合

- [ ] Export PNG（html2canvas）
- [ ] Export 圖像 prompt
- [ ] AI 文案輔助（GPT 寫文案變體）
- [ ] AI 生圖整合（imageHint → 圖片素材）
- [ ] Kiwa Tasks 整合（task.metadata 儲存草稿）
- [ ] 多客戶模板（漁讚、時時醫美、往山裡走等）
