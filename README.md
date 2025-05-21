# 🎉 公文時效計算器（GWTimer）

這是一套專為計算公文辦理時效的網頁工具；根據不同的辦理情形及起迄時間，並參考政府行事曆，自動計算處理時數與換算處理日數。

👉 [線上使用連結（GitHub Pages）](https://volache.github.io/GWTimer)


## 📦 功能特色

- **四種辦理情形**：
  - 📁 來文存查、
  - 📬 來文函復、
  - 📝 創簽存查、
  - 📤 創稿發文。
- **彈性時間選擇**：
  - 使用 Flatpickr 日期時間選擇器設定公文辦理的起始與結束時間。
- **自動載入政府行事曆**：
  - 透過 [ruyut/TaiwanCalendar](https://github.com/ruyut/TaiwanCalendar) 獲取政府行事曆資料，判斷國定假日與補班日。
- **自訂額外停班日**：
  - 可手動輸入因颱風等因素導致的額外停班日，並儲存於瀏覽器供下次使用。
- **時效計算**：
  - 以「日、小時、分鐘」方式顯示處理時數，並根據特定規則轉換為處理日數。
- **詳細時數明細**：
  - 清楚列出公文辦理期間每日的狀態及該日的處理時數。
- **內建操作說明**：
  - 提供詳細的彈出式操作說明，方便使用者快速上手。


## 🖥 技術架構

- [Vue 3](https://vuejs.org/)：前端框架。
- [Tailwind CSS](https://tailwindcss.com/)：UI 樣式設計。
- [Flatpickr](https://flatpickr.js.org/)：日期時間選擇器。
- [TaiwanCalendar API](https://github.com/ruyut/TaiwanCalendar)：政府行事曆資料。


## 💻 本機安裝運行

1.  下載專案至本機：
    ```bash
    git clone https://github.com/volache/GWTimer.git
    ```
2.  進入專案目錄：
    ```bash
    cd GWTimer
    ```
3.  使用瀏覽器直接開啟 `index.html`。


## 📅 行事曆資料來源

本工具使用的政府行事曆資料來自 GitHub 上的 [ruyut/TaiwanCalendar](https://github.com/ruyut/TaiwanCalendar) 專案，該專案提供了台灣政府行事曆的 JSON 格式資料；感謝其維護與分享。
