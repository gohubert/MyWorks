# 我的網頁作品集 (MyWorks)

> **楊宏文（楊老師 / Hubert Yang）**｜AI365 品牌創辦人 • 企業生成式 AI 導入顧問 • 25 年資訊人才培訓專家

本專案收錄透過 **AI365 工作流**、**Spec-Driven（規格驅動開發）** 與 **Vibe Coding** 打造的單檔網頁應用程式（Single-File Web Apps）與個人顧問品牌頁。所有工具皆採用 **100% 瀏覽器本機端運算架構**，資料不上傳外部伺服器，兼顧資訊安全、個資合規與跨裝置（手機優先 Mobile-First）操作體驗。

---

## 📂 專案目錄結構

```text
MyWorks/
├── index.html                              # 作品集首頁（手機優先設計，含作品目錄、小圖卡與關於我）
├── about/
│   └── index.html                          # 關於我：楊宏文老師完整企業 AI 導入顧問履歷頁
├── apps/
│   ├── data-deidentification-tool.html     # 作品 1：企業資料去識別化工具（R4 楊老師版）
│   ├── overtime-analysis-dashboard.html    # 作品 2：加班工時診斷儀表板
│   ├── sales-performance-dashboard.html    # 作品 3：銷售營運互動分析儀表板
│   └── tarot-reading-78-cards.html         # 作品 4：星語塔羅｜78 張塔羅與繁體中文深度解牌
├── assets/
│   └── myphoto.jpg                         # 個人形象照
└── music/
    └── music-1.mp3                         # 網站背景配樂
```

---

## 🚀 作品一覽

### 1. 企業資料去識別化工具 (`apps/data-deidentification-tool.html`)
* **簡介**：專為企業打造的純前端離線資料脫敏工具，全程於本機瀏覽器運算、不上傳雲端。支援 Excel 多工作表（`.xlsx`）與 `.csv` 批次處理，提供跨表一致的擬真假名化、遮罩、泛化、等比例縮放與數值微擾等七大技術，並可匯出還原對照表，兼顧資料分析價值與個資合規安全。
* **核心 API 與技術**：`File & FileReader API`、`HTML Drag and Drop API`、`TextDecoder (UTF-8 / Big5)`、`DOMParser (XML)`、`Blob & URL.createObjectURL`、內嵌 `ExcelJS` 與 `fflate` 解壓引擎。
* **應用場景**：企業將含個資或營業秘密之報表交付外部顧問、上傳 AI 分析前之安全脫敏、跨部門數據共享、系統測試擬真資料生成，以及教育訓練範例製作。

### 2. 加班工時診斷儀表板 (`apps/overtime-analysis-dashboard.html`)
* **簡介**：專為人資與管理層設計的本機端工時診斷系統，無須外部套件即可直接解析 XLSX 與 CSV。內建資料健檢與智慧欄位對應，透過四大分析模組自動計算部門趨勢迴歸、吉尼係數集中度、法規超標分級、人力缺口替補比與員工負荷風險評分，一鍵產出根因診斷報告。
* **核心 API 與技術**：`DecompressionStream API (deflate-raw)`、`DataView & TypedArray`（ZIP 中央目錄解析）、`DOMParser (XML)`、`File & Blob URL API`、動態 `SVG` 視覺化、`CSS Print` 列印排版。
* **應用場景**：HR 勞基法加班工時合規稽核、部門長期高工時預警、未核准加班黑數排查、部門人力編制缺口評估，以及異常缺勤與過勞高風險員工關懷名單篩選。

### 3. 銷售營運互動分析儀表板 (`apps/sales-performance-dashboard.html`)
* **簡介**：具備嚴格 CSP 安全防護的零依賴銷售 BI 儀表板，拖入 Excel 或 CSV 即可在瀏覽器內自動完成多表關聯與資料勾稽健檢。涵蓋業績區域達成率、產品毛利侵蝕拆解、客戶柏拉圖 ABC 與鯨魚曲線、假大戶識別及業務員績效象限，自動生成經營摘要與異常診斷。
* **核心 API 與技術**：`DecompressionStream API`、`DataView & BigUint64 (ZIP64 解析)`、`DOMParser (XML)`、`File & Drag-and-Drop API`、`Content-Security-Policy (CSP)`、`window.print()` 診斷報告。
* **應用場景**：企業經營層月度與季度業績復盤、低毛利與虧損訂單根因追蹤、高營收低毛利「假大戶」篩查、業務員未核准折扣稽核與銷售目標達成率管理。

### 4. 星語塔羅｜78 張塔羅與深度解牌 (`apps/tarot-reading-78-cards.html`)
* **簡介**：收錄完整 78 張偉特塔羅大阿爾克那與四元素牌組的離線互動占卜應用。採用密碼學等級亂數進行洗牌與正逆位抽取，支援單張指引、三張時間流與五張深度剖析牌陣，結合感情、工作、財務等六大主題，自動生成結構化繁體中文牌義解析、反思提問與具體行動建議。
* **核心 API 與技術**：`Web Crypto API (crypto.getRandomValues)`、`Web Storage API (localStorage)`、`Clipboard API (navigator.clipboard)`、`ARIA Live` 無障礙狀態通知。
* **應用場景**：個人日常決策換位思考、職涯與專案盲點探索、人際與感情關係梳理、靜心自我對話，以及無網路環境下隨時可用的行動端象徵性牌卡工具。

---

## 👤 關於作者：楊宏文（楊老師 / Hubert Yang）

* **品牌理念**：創立「**AI365**」工作流品牌，強調將生成式 AI 融入日常工作流程（AI Workflow），建立**可制度化（AI Governance）**、**可衡量（AI ROI）**、**可擴張（Scalable AI）**的企業級 AI 能力。
* **專業實績**：
  * **25+ 年**資訊專業就業技能培訓經驗
  * **1,000+ 名**學員成功輔導轉職為工程師
  * **800+ 名**學員通過 ITS AI / CCS GAI 國際認證
  * **5.92 / 6** 大型企業（中華電信等）生成式 AI 實作內訓平均滿意度

---

## 💻 使用方式

1. 直接克隆或下載本專案：
   ```bash
   git clone https://github.com/gohubert/MyWorks.git
   ```
2. 直接以瀏覽器開啟主目錄下的 `index.html`，或透過 GitHub Pages 線上瀏覽所有作品。
