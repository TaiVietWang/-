# 博客來爬蟲 Notebooks（books.com.tw crawlers）

這個專案整理了四支 Jupyter Notebook，分別用於從 **博客來（books.com.tw）** 抓取不同欄目的書籍清單。  
> 僅供學術研究與技術交流，請務必遵守目標網站的 **服務條款** 與 **robots.txt**，避免高頻請求造成站方壓力。

## 📁 專案結構
```
.
├─ notebooks/
│  ├─ 博客來即將出版0923.ipynb      # 即將出版（Upcoming）
│  ├─ 博客來預購0923.ipynb          # 可預購（Pre-order）
│  ├─ 博客來獨家0923.ipynb          # 博客來獨家（Exclusive）
│  └─ 博客來新書清單0923.ipynb      # 新書清單（New Releases）
├─ requirements.txt
├─ .gitignore
├─ LICENSE
└─ README.md
```

## 🚀 快速開始
### 1) 下載或複製專案
```bash
git clone https://github.com/<your-username>/<your-repo>.git
cd <your-repo>
```

### 2) 建立虛擬環境（建議）
```bash
python -m venv .venv
# Windows
.venv\Scripts\activate
# macOS/Linux
source .venv/bin/activate
```

### 3) 安裝依賴
```bash
pip install -r requirements.txt
```

### 4) 執行 Notebook
- 使用 VS Code、Jupyter Lab 或 `jupyter notebook` 開啟 `notebooks/` 下的 `.ipynb` 檔即可。
- 若需要瀏覽器自動化（例如 Selenium/Playwright），請自行安裝對應驅動與瀏覽器，並依 Notebook 內註解調整。

## 📌 重要注意事項
- **合法合規**：請事先閱讀並遵守目標網站的 **Terms of Service** 與 **robots.txt**。
- **頻率控制**：加入 `time.sleep()`、**指數退避** 以及 **重試** 機制，避免對站方造成影響。
- **隱私與金鑰**：請勿將帳密、Cookie、API Key 明文寫入程式；如需設定，請改用 `.env` 檔與環境變數管理。`.env` 已在 `.gitignore` 排除。
- **資料用途**：僅供研究與學習，商業使用請自行確認合法性。

## 🙋‍♀️ 我可以怎麼貢獻？
- 發 Issue 回報錯誤或提出改進建議
- 發 Pull Request 一起改善程式、補充文件與測試

## 📝 授權
本專案以 **MIT License** 授權。

---

## English (brief)
This repository contains four Jupyter notebooks for scraping different book lists from **books.com.tw** (Upcoming, Pre-order, Exclusive, and New Releases).  
**For research/educational purposes only.** Please respect the website's Terms of Service and robots.txt, and rate-limit your requests.
