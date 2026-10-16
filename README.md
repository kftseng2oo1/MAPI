# 萬用 API 連結申請手冊

開發者常用 API 的申請流程、費用結構與程式碼範例，並可在本機記錄自己的 Key 與申請狀態。

**線上使用**：https://kftseng2oo1.github.io/MAPI/

## 分類
- 📡 通訊類：LINE Messaging API 等
- 🤖 AI／運算類：Anthropic Claude、Google Gemini、OpenAI、Hugging Face
- 🗺 地圖／地標類：Google Maps、OpenStreetMap Nominatim、Leaflet
- 🗄 後端服務類：Cloudflare Workers、Firebase、Notion、GitHub
- ✉️ 通知／簡訊類：SendGrid、Twilio
- 🔧 其他工具類：Imgur、SheetJS 等

## 主要功能
- 每張卡片含申請網址、步驟、費用、程式碼範例（一鍵 COPY）
- 可切換「直連」或經 `arcar.kftseng2oo1.workers.dev` 代理的範例寫法
- 「金庫」欄位把自己的 Key 存在本機（IndexedDB），點擊標記是否已申請
- 搜尋過濾卡片

## 技術與依賴
- 單檔 HTML PWA（`index.html` 內含全部 HTML/CSS/JS），`manifest.json` + `sw.js` 提供安裝到主畫面與離線快取。
- Key 只存在瀏覽器本機，不會上傳
