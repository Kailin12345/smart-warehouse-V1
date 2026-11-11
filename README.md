# 📦 智慧儲存庫與食品過期管理系統 (Smart Warehouse & Expiry Management)

這是一個基於 **純前端網頁 (HTML / JavaScript)** 與 **行動裝置本地運算** 的智慧儲存庫與食品過期管理系統。不需要任何後端伺服器或複雜硬體，打開瀏覽器或透過 NFC 貼紙即可隨時隨地管理家中物品與食品有效期限！

---

## ✨ 核心功能特色

* **📦 動態儲存庫與儲位管理：** 自由建立不同分類（如：衣櫃、工具箱、食品櫃），並支援儲位細分。
* **🏷️ NFC 快速導航：** 結合 NFC 貼紙與網址參數（Query Parameters），手機輕觸即可秒開對應的儲存庫。
* **✨ 手機本地 AI 影像辨識：** 整合 **TensorFlow.js (MobileNet)**，直接利用手機晶片進行離線影像辨識，自動帶入物品名稱。
* **📷 商品條碼掃描：** 內建 `Html5-Qrcode` 掃描器，快速讀取商品條碼。
* **⏳ 食品有效期限追蹤：** 記錄食品入庫與有效期限，隨時透過「現有庫存清單」掌握狀態，避免過期浪費。
* **💾 本地端優先 (Local-First)：** 所有資料與照片皆儲存在瀏覽器的 `LocalStorage` 中，隱私安全且完全免上雲端。

---

## 🛠️ 技術架構

* **前端介面：** 原生 HTML5, CSS3, JavaScript (Vanilla JS)
* **AI 辨識模型：** TensorFlow.js & MobileNet (前端瀏覽器運算)
* **條碼掃描：** Html5-Qrcode 函式庫
* **資料儲存：** Browser LocalStorage
* **部署平台：** GitHub Pages (免費靜態網頁託管)

---

## 🚀 快速開始與使用方式

1. **直接線上使用：**
   * 請造訪本專案的 GitHub Pages 網址：[https://kailin12345.github.io/smart-warehouse/](https://kailin12345.github.io/smart-warehouse/) （請替換為你的實際網址）
2. **手機桌面捷徑：**
   * 使用手機瀏覽器開啟網頁後，點擊選單選擇 **「加到主畫面」**，即可獲得如同 App 般的流暢體驗。
3. **搭配 NFC 貼紙：**
   * 將帶有特定參數的網址寫入 NTAG NFC 貼紙中：
     * 範例（食品櫃）：`https://你的帳號.github.io/smart-warehouse/?storage=pantry`
     * 範例（特定抽屜）：`https://你的帳號.github.io/smart-warehouse/?storage=toolbox&loc=抽屜-A1`

---

## 📌 畫面預覽與操作流程
1. **入庫登記：** 選擇或新增儲存庫 ➔ 掃描條碼或拍照 ➔ 執行本地 AI 辨識 ➔ 填寫過期日與數量 ➔ 儲存。
2. **庫存清單：** 切換至上方頁籤即可檢視所有物品縮圖、儲位與過期狀況。
