# 博客來爬蟲 Notebooks（books.com.tw crawlers）

一組用 Python 撰寫的 博客來書籍爬蟲 Jupyter Notebooks，可自動抓取即將出版、預購、獨家、新書清單等書籍資訊，並輸出為結構化資料（如 CSV），方便後續分析與應用。僅供學術研究與技術交流，請務必遵守目標網站的服務條款與 robots.txt，並適當控制請求頻率。

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
A set of Python Jupyter Notebooks for scraping book data from books.com.tw, covering Upcoming, Pre-order, Exclusive, and New Releases categories. The scripts output structured data (e.g., CSV) for easy analysis. For research and educational purposes only – please respect the site's Terms of Service, robots.txt, and apply proper rate limiting.
