# Internet-programming-lunch-picker
一款可以幫助你挑選午餐的小助理，解決您勞心耗神的午餐選擇困難症
# 🍱 LunchPicker
**「欸午餐要吃什麼？」抽籤器 – 網際網路程式設計第五組專案**

---

## 🧭 專案簡介 | Project Overview

每天午餐都陷入「吃什麼」的無限循環？  
**LunchPicker** 幫你解決選擇障礙！  
輸入地點與想吃的餐點類型，系統會自動幫你從附近餐廳中**隨機抽出一家**，  
讓你的午餐選擇更輕鬆、有趣。

> “Stop struggling — let LunchPicker decide for you!”

---

## 💡 動機與設計原因 | Motivation

現代人每天面臨三大問題：
1. 不知道中午要吃什麼 🍛  
2. 每次都吃同一家，生活缺乏新鮮感 😩  
3. 想吃的餐廳太多，猶豫不決 😵‍💫  

**LunchPicker** 讓使用者：
- 根據地點與餐點類型篩選  
- 隨機抽出一家餐廳  
- 一鍵導向 Google Maps，直接導航！

---

## 🧰 使用工具與技術架構 | Tech Stack

| 類別 | 技術 / 工具 |
|------|--------------|
| 前端 | HTML, CSS, JavaScript, React |
| API串接 | OpenStreetMap Nominatim API, Overpass API |
| （延伸） | Google Geocoding API, Geolocation API |
| 設計工具 | Figma |
| 開發框架 | React Components + JavaScript 模組化架構 |

---

## 🗺️ 系統流程 | System Flow

1. **輸入地點**  
   使用者輸入地址或地標 → Nominatim / Google Geocoding 轉為經緯度  
2. **設定篩選條件**  
   可調整搜尋半徑（500m–5km）與餐點類型（中式 / 日式 / 西式 / 速食等）  
3. **呼叫 Overpass API**  
   根據經緯度與餐點類型查詢附近餐廳資料  
4. **隨機抽籤**  
   以 `Math.random()` 抽出一家餐廳  
5. **顯示結果**  
   顯示餐廳名稱、地址與類型  
   點擊後可直接跳轉 Google Maps  

---

## 🧩 API 資料來源 | APIs

| 名稱 | 用途 | 說明 |
|------|------|------|
| [OpenStreetMap Nominatim API](https://nominatim.openstreetmap.org/) | 地理編碼 | 將地址轉為經緯度 |
| [Overpass API](https://overpass-api.de/) | 餐廳資料查詢 | 查詢地點附近的商家資料 |
| (可選) Google Geocoding API | 地理編碼備援 | 付費方案、每日限額 |
| (延伸) Geolocation API | 自動定位 | 自動偵測使用者位置 |

---

## ✨ 功能特色 | Features

- 🔍 地址 / 地標輸入  
- 🍜 餐點類型與距離篩選  
- 🎯 隨機餐廳抽籤  
- 🗺️ Google Maps 導航連結  
- 🎡 動態動畫轉盤效果（以 GSAP 製作）  

---

## 🚀 延伸與未來發展 | Future Development

- 🛵 一鍵導向 Uber Eats / Foodpanda 訂餐頁  
- 💬 社群分享與評價系統  
- 👥 「一起吃飯」揪團功能  
- 🧠 智慧推薦相似餐廳（同區域 / 同類型）  

---

## 🧑‍💻 團隊成員 | Team Members

| 學號 | 姓名 | 負責項目 |
|------|------|----------|
| 科技115 | 李怡安 | 前端開發、API 串接 |
| 科技116 | 盧姵帆 | 介面設計、互動邏輯 |
| 科技117 | 王泰崴 | React 組件整合 |
| 科技117 | 周均翰 | 資料處理與演算法 |
| 科技117 | 溫竣閔 | 視覺設計與動畫 |
| 科技117 | 茬遠淳 | 系統測試與文檔撰寫 |

---

## 📸 預期成果 | Expected Results

- 可互動式午餐抽籤介面  
- 附地圖與即時導航功能  
- 有趣的使用者體驗與動畫效果  
