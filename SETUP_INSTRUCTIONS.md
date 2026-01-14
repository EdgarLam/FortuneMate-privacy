# 設定指南：部署隱私權政策到 GitHub Pages

## 📋 步驟說明

### 第一步：在 GitHub 創建新的公開儲存庫

1. **前往 GitHub**
   - 訪問：https://github.com/new

2. **填寫儲存庫資訊**
   - **Repository name（儲存庫名稱）：** `fortunemate-privacy`
   - **Description（描述）：** `Privacy Policy for FortuneMate App`
   - **可見性：** 選擇 **Public**（公開）✅
   - **不要勾選** "Initialize this repository with a README"

3. **點擊 "Create repository"**

### 第二步：推送檔案到新儲存庫

在終端機中執行以下指令（已經在 `privacy-repo-setup` 資料夾中準備好）：

```bash
# 1. 進入 privacy-repo-setup 資料夾
cd /Users/edgar/FortuneMate/privacy-repo-setup

# 2. 初始化 Git 儲存庫
git init

# 3. 添加所有檔案
git add .

# 4. 提交檔案
git commit -m "Initial commit: Add privacy policy page"

# 5. 設定遠端儲存庫（請替換成您的 GitHub 用戶名）
git remote add origin https://github.com/EdgarLam/fortunemate-privacy.git

# 6. 推送到 GitHub
git branch -M main
git push -u origin main
```

### 第三步：啟用 GitHub Pages

1. **前往儲存庫設定**
   - 訪問：https://github.com/EdgarLam/fortunemate-privacy/settings/pages

2. **設定 GitHub Pages**
   - 在 **"Source"** 部分
   - 選擇 **"main"** 分支
   - 資料夾選擇 **"/ (root)"**
   - 點擊 **"Save"** 按鈕

3. **等待部署**
   - GitHub 會自動部署（通常 1-2 分鐘）
   - 頁面會顯示部署狀態

4. **取得公開 URL**
   - 部署完成後會顯示：
   - `https://edgarlam.github.io/fortunemate-privacy/privacy-policy.html`

### 第四步：在 App Store Connect 使用

1. 登入 App Store Connect
2. 前往您的應用程式
3. 在「App 隱私權」部分
4. 輸入隱私權政策 URL：
   ```
   https://edgarlam.github.io/fortunemate-privacy/privacy-policy.html
   ```

## ✅ 完成！

您的隱私權政策現在已經公開可訪問，可以用於 Apple App Store 提交。

## 🔄 未來更新

如需更新隱私權政策：

1. 修改 `privacy-policy.html`
2. 提交並推送到 GitHub
3. GitHub Pages 會自動更新（通常幾分鐘內）

---

**注意：** 請確保將上述指令中的 `EdgarLam` 替換為您實際的 GitHub 用戶名（如果不同的話）。
