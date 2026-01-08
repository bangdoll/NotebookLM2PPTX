# NotebookLM 簡報工具箱 (NotebookLM2PPTX)

這是一個強大的 AI 逆向工程工具，專為 NotebookLM PDF 簡報打造。它整合了 PDF 解析、AI 智慧去字與 PPTX 合併功能，讓您能輕鬆將靜態 PDF 轉換為可編輯的 PPTX 簡報。

## 主要功能

### 1. PDF 高精細解析 & 視覺還原
- **PDF 匯入**：支援拖放或點擊上傳 PDF 檔案。
- **高解析度渲染**：將 PDF 頁面轉換為高解析度圖像，保留原始排版細節。
- **AI 視覺還原**：利用最新 **Gemini 3 Flash Preview** 模型進行 OCR 識別，速度更快更精準。

### 2. AI 圖片智慧去字
- **圖片去文字工作台**：專門針對簡報背景圖設計的去字功能。
- **動態無限槽位**：不再受限於固定數量，系統會根據匯入的圖片數量自動增加工作槽位，支援大量批次處理。
- **AI 填補技術**：整合頂尖的 **Gemini 3 Pro Image Preview** 模型，移除文字後的背景填補效果更自然、細節更豐富。
- **一鍵導出**：處理完成的乾淨背景圖可直接匯出為 PPTX。

### 3. PPTX 魔法合併
- **XML 層級合併**：將「純文字 PPTX」的內容完美移植到「背景圖 PPTX」上。
- **保留排版**：精確保留文字的位置、樣式與動畫設定。
- **操作簡單**：只需上傳兩個檔案，系統自動完成合併並提供下載。

## 安全性設計

- **API Key 本地存儲**：您的 Google Gemini API Key 僅存儲在瀏覽器的 `localStorage` 中，**絕不**會傳送到任何第三方伺服器，確保您的額度與帳號安全。
- **安全設定介面**：提供直觀的設定視窗，方便您管理 API Key。
- **智慧速率控制**：
  - **🐢 免費版模式**：自動限制請求速度 (15 RPM)，避免觸發 429 錯誤，穩定可靠。
  - **🚀 付費版模式**：開啟多線程高併發處理，充分利用 Pay-as-you-go 的高速額度。

## 使用技術

- **前端核心**：原生 JavaScript (Vanilla JS) + HTML5
- **樣式框架**：Tailwind CSS (透過 CDN引入)
- **PDF 處理**：PDF.js
- **PPTX 生成**：PptxGenJS
- **PPTX 解析/壓縮**：JSZip & FileSaver.js
- **AI 模型**：Google Gemini API (gemini-3-flash-preview, gemini-3-pro-image-preview)

## 授權

MIT License
