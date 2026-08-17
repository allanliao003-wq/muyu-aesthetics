# 莯遇美學・清水沙鹿店 官網

台中沙鹿「莯遇美學」全身SPA／岩盤浴／身體調理館的品牌形象官網。純靜態網頁（HTML / CSS / JavaScript），沒有使用任何前端框架，做法比照 0度造型工作室官網。

## 線上連結

| 項目 | 網址 |
|---|---|
| 正式網站 | https://muyu-aesthetics.vercel.app |
| GitHub Repo | https://github.com/allanliao003-wq/muyu-aesthetics |

## 技術架構

- 純 HTML + CSS + JavaScript，無框架、無建置流程、無 npm 依賴
- 部署：Vercel，已連接 GitHub repo，push 到 `main` 分支會自動重新部署上線

## 檔案結構

```
muyu-aesthetics/
├── index.html   # 頁面所有內容（結構＋文案）
├── style.css     # 樣式：設計 tokens、版面、動態效果
└── script.js      # 互動效果：選單、捲動進場動畫、數字計數
```

## 本機預覽

```bash
cd muyu-aesthetics
python3 -m http.server 8000
```

瀏覽器開 `http://localhost:8000` 即可預覽。

## 內容怎麼改

| 想改什麼 | 去哪裡改 |
|---|---|
| 服務項目文字 | `index.html` 內 `<section class="services">` |
| 品牌故事文字 | `index.html` 內 `<section class="about">` |
| 預約資訊（地址／營業時間／連結） | `index.html` 內 `<section class="info">` |
| 顏色、字體、間距 | `style.css` 最上方 `:root { ... }` 的 CSS 變數 |
| 選單、動畫行為 | `script.js` |

## 目前用的資料來源與待確認事項

- 品牌名稱「莯遇美學」為使用者確認採用的字（注意：IG／FB 頭像截圖上實際顯示的字是「茉遇」，兩者不同，若之後要對外印刷物或其他通路露出，建議跟業主再三確認正式字型）
- 服務項目（全身SPA／岩盤浴／深層調理／肌膚管理／孕婦按摩）與地址（台中市沙鹿區星海路35號）取自 IG／FB 截圖
- 營業時間 09:30–21:30 取自 Facebook 頁面截圖當下顯示的「營業中」狀態，網站上已註明「請以官方最新公告為準」，避免資訊錯誤
- LINE 官方帳號連結已附上（使用者提供）；Instagram 連結為 @mumeet_sl（截圖上的帳號）
- **沒有 Facebook 粉專的網址**，截圖只有頁面畫面、没有網址列，所以官網上這段只用文字提示「歡迎在 Facebook 搜尋」，沒有做成連結。之後有正確網址可以直接補上
- 服務項目**不放價格**（比照 0度造型工作室的作法：沒把握的資訊不寫，一律標示「歡迎透過 LINE 洽詢」）
- Hero 與各區塊視覺目前用色塊／漸層／字體排版做出質感，**沒有使用任何店內實拍照**（避免引用來路不明或可能失效的圖片網址）。之後有店內實拍照片，可以直接把 `.hero` 的漸層背景換成實景照片，質感會更接近截圖裡的溫暖木質調風格
