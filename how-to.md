# 作業提交流程說明

本作業目的是讓學生熟悉 GitHub 的基本操作流程，包括 fork、clone 和 pull request。

## 作業提交步驟

### 1. Fork 此專案

1. 前往課程的 GitHub 專案頁面：https://github.com/NCUE-CS-RL-2026-Spring/homework-0
2. 點擊頁面右上角的 **Fork** 按鈕
3. 選擇你的 GitHub 帳號作為 fork 的目標
4. 等待 fork 完成，你會在自己的 GitHub 帳號下看到此專案的副本

### 2. Clone 專案到本地

```bash
git clone https://github.com/<你的-username>/homework-0.git
cd homework-0
```

請將 `<你的-username>` 替換為你的 GitHub 使用者名稱。

### 3. 填寫 README.md

使用你喜歡的文字編輯器打開 `README.md`，填寫以下內容：

- 學號
- 姓名
- 自我介紹
- 為什麼選這堂課

### 4. 提交變更

```bash
git add README.md
git commit -m "完成作業 0：填寫個人資訊"
```

### 5. 推送到你的 GitHub

```bash
git push origin main
```

如果預設分支是 `master`，請使用：
```bash
git push origin master
```

### 6. 建立 Pull Request

1. 前往你自己 fork 的專案頁面（`https://github.com/<你的-username>/homework-0`）
2. 點擊 **Contribute** → **Open pull request** 按鈕
3. 確認分支資訊：
   - base: `NCUE-CS-RL-2026-Spring:main`
   - compare: `<你的-username>:main`
4. 在標題中填寫：`Homework 0 - <你的姓名> - <你的學號>`
5. 在內容中可以簡單說明你的作業完成情況
6. 點擊 **Create pull request** 送出

## 常見問題

### 如何檢查目前分支？

```bash
git branch
```

### 如何切換到 main 或 master 分支？

```bash
git checkout main
# 或
git checkout master
```

### 如何查看遠端 repository？

```bash
git remote -v
```

### 如果需要更新本地專案與最新的課程版本同步？

在 fork 的專案中添加上游遠端：
```bash
git remote add upstream https://github.com/NCUE-CS-RL-2026-Spring/homework-0
git fetch upstream
git merge upstream/main
```

## Markdown 基本語法

- 標題：`# 一級標題`、`## 二級標題`
- 粗體：`**粗體文字**`
- 斜體：`*斜體文字*`
- 列表：`- 項目` 或 `1. 編號項目`
- 連結：`[連結文字](URL)`
- 區塊程式碼：\`\`\`語言\`\`\`

祝作業順利！如有問題請聯繫助教或課程助教團隊。
