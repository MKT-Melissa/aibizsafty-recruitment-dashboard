# 生生護動 招生說明會成效分析 Dashboard - 設置指南

## 🚀 快速開始

### 方式一：線上使用（推薦）
直接訪問 GitHub Pages 網址，無需任何設置：
**https://mkt-melissa.github.io/aibizsafty-recruitment-dashboard/**

### 方式二：本地開發

#### 步驟 1: 克隆儲存庫
```bash
git clone https://github.com/MKT-Melissa/aibizsafty-recruitment-dashboard.git
cd aibizsafty-recruitment-dashboard
```

#### 步驟 2: 創建 config.js 文件
在項目根目錄創建 `config.js` 文件，內容如下：

```javascript
// Airtable Configuration
// 注意：請勿將此檔案提交到版本控制系統
// NOTE: Do not commit this file to version control

const AIRTABLE_CONFIG = {
    TOKEN: "your_airtable_token_here",
    BASE_ID: "your_base_id_here",
    TABLE_ID: "your_table_id_here"
};
```

#### 步驟 3: 替換敏感信息
用您的 Airtable 資訊替換以下部分：
- `TOKEN`: 您的 Airtable Personal Access Token
- `BASE_ID`: 您的 Base ID
- `TABLE_ID`: 您的 Table ID

#### 步驟 4: 打開 Dashboard
用瀏覽器打開 `index.html` 文件，即可看到即時同步的 Dashboard。

## 📝 重要說明

- **config.js 文件**: 此文件包含敏感信息（API Token），已添加到 `.gitignore`，不會被提交到版本控制系統。
- **線上版本**: GitHub Pages 部署的線上版本無法使用 API 集成（CORS 限制），但靜態版本 `static-version.html` 可作為備選。
- **安全性**: 請勿在版本控制中提交 Token 或其他敏感信息。

## 🔧 功能特性

- ✅ 即時同步 Airtable Pipeline 數據
- ✅ 自動計算 MQL = SQL + 競品 + 合作夥伴 + 其他
- ✅ 園區篩選與動態圖表
- ✅ KPI 展示與數據表格
- ✅ 轉換率趨勢分析

## 📞 支持

如有任何問題，請檢查：
1. config.js 文件是否正確創建
2. Airtable Token 是否有效
3. Base ID 和 Table ID 是否正確
4. 瀏覽器控制台是否有錯誤信息
