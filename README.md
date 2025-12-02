# 🐶 妙麗歲數計算機

這個專案是一個簡單的靜態網站（只有 `index.html`），用來計算狗狗年齡與換算成人類年齡。

## 在 GitHub Pages 上部署
以下步驟可將此網站公開並自動部署到 GitHub Pages：

1. 在 GitHub 上建立一個新的 repository（同名或不同皆可）。
2. 如果本機尚未加入遠端，請在本機資料夾初始化 git 並加入遠端：

```powershell
# 進入專案資料夾
Set-Location 'c:\Users\h4030\Desktop\Day 08 - 除了 HTML、CSS，還有 JS！'

# 如果尚未初始化 git
git init
git add .
git commit -m "Initial commit"

# 將遠端 repo 指定為 origin（改成你自己的 repo URL）
git remote add origin https://github.com/<你的帳號>/<你的-repo>.git
git branch -M main
git push -u origin main
```

3. 本專案已包含一個 GitHub Actions workflow (`.github/workflows/pages.yml`)，會在每次 push 到 `main` 時自動部署靜態內容到 GitHub Pages（官方 Pages action）。

4. 如果使用手動設定（不使用 workflow），在 GitHub repo 的 "Settings > Pages" 中選擇 Branch 和 /（root）作為來源。

5. 部署成功後，GitHub 頁面會顯示你站點的網址（通常是 `https://<你的帳號>.github.io/<你的-repo>/` ）。

## 額外說明
- `.nojekyll`：避免 GitHub Pages 使用 Jekyll 處理（已新增於此 repo）。
- 若想更精細化或自訂網址（CNAME），可新增 `CNAME` 檔案。

祝你部署順利！需要我幫你自動設定或示範推送遠端嗎？
