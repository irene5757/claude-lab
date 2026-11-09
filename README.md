# Irene — 平面設計師作品集 Landing Page

自由接案平面設計師 Irene 的個人作品集單頁網站（Landing Page），以「夜空星光」為視覺主題，介紹設計服務、展示精選作品，並引導訪客來信洽談合作。

## 網站功能

- **導覽列**：固定於頂部（sticky），帶毛玻璃效果，並顯示目前的接案檔期狀態。
- **英雄區塊（Hero）**：主標語、個人簡介，以及「與我聯繫」「觀看作品」兩個行動按鈕；下方列出服務項目（Brand Identity、Editorial、Packaging、Art Direction）。
- **精選作品**：三張作品卡片，分別是品牌識別、編排設計與包裝設計，各附設計概念說明；滑鼠移入時有浮起與圖示旋轉效果。
- **聯絡區塊**：一鍵開啟 Email（`mailto:`）聯絡設計師。
- **頁尾**：版權資訊與快速連結（作品、聯絡、回到頂部）。
- **動態效果**：多層星空背景閃爍與漂移、流星動畫、進場淡入，以及捲動到區塊時的淡入效果。
- **RWD 響應式設計**：
  - 960px 以下：作品改為兩欄排列。
  - 720px 以下（手機版）：作品單欄垂直排列、標題縮小、側邊留白 16px，連結點擊區域至少 44px 高，方便觸控。
  - 420px 以下：按鈕改為滿版寬度，精簡導覽列資訊。
- **無障礙**：支援鍵盤焦點樣式（`:focus-visible`），並在使用者開啟「減少動態效果」（`prefers-reduced-motion`）時關閉動畫。

## 使用技術

- **HTML5**：語意化標籤（`header`、`main`、`section`、`article`、`footer`）。
- **CSS3**：CSS 變數、Flexbox、Grid、`clamp()` 流體字級、漸層與 `backdrop-filter`、`@keyframes` 動畫、Media Queries。
- **內嵌 SVG**：Logo 與作品圖示皆以 SVG 繪製，不需額外圖片檔。
- **Google Fonts**：Inter、Noto Sans TC、Cormorant Garamond。
- 少量原生 JavaScript（`IntersectionObserver`）處理捲動淡入效果，無任何框架或建置工具。

## 如何用瀏覽器開啟

本專案是純靜態網頁，不需要安裝任何套件或啟動伺服器。

1. 下載或 clone 此專案：
   ```bash
   git clone https://github.com/irene5757/claude-lab.git
   ```
2. 進入專案資料夾，直接用滑鼠**雙擊 `index.html`**，即會以預設瀏覽器開啟。
3. 或者在瀏覽器中按 `Ctrl + O`（macOS 為 `Cmd + O`），選擇 `index.html` 開啟。

> 提示：想查看手機版效果，可在瀏覽器按 `F12` 開啟開發者工具，再按 `Ctrl + Shift + M` 切換到裝置模擬模式。

## 檔案結構

```
claude-lab/
├── index.html   # 網站主頁（HTML + 內嵌 CSS）
├── note.txt     # 筆記
└── README.md    # 專案說明
```
