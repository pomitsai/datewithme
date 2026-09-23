# 淳淳的約會邀請網頁

這是一個不需要安裝套件的靜態網站，已包含：

- 手機、平板與電腦響應式版面
- 五頁動畫場景與角色素材
- 姓名必填驗證
- 日期、接送時間與飲料互動
- Google 表單自動送出功能

## 檔案結構

```text
date-invitation-github/
├── index.html
├── .nojekyll
├── README.md
└── assets/
    ├── maruko-bow.png
    ├── scene-welcome-v2.png
    ├── scene-date-v2.png
    ├── scene-pickup-v2.png
    ├── scene-drink-v2.png
    └── scene-thanks-v2.png
```

## 部署到 GitHub Pages

1. 在 GitHub 建立一個新的公開或私人 Repository。
2. 將本資料夾內的所有檔案上傳到 Repository 根目錄。請確認 `index.html` 位於最上層，不要只上傳 ZIP。
3. 進入 Repository 的 `Settings` → `Pages`。
4. 在 `Build and deployment` 中將 `Source` 設為 `Deploy from a branch`。
5. Branch 選擇 `main`，資料夾選擇 `/ (root)`，按下 `Save`。
6. 等候數分鐘後，GitHub 會提供網站網址。

## Google 表單設定

Google 表單回應端點與四個欄位識別碼已寫在 `index.html` 的 `FORM_CONFIG` 中：

- 你是誰？
- 日期
- 上車時間
- 隨車飲料

若日後刪除並重建 Google 表單題目，欄位識別碼可能改變，需同步更新 `FORM_CONFIG`。

## 注意事項

- GitHub Pages 上的網站內容與圖片通常可被瀏覽者下載。
- Google 表單欄位識別碼會出現在網頁原始碼中；它不是密碼，但不要在網頁中放入任何帳號密碼或 API 金鑰。
- 網頁使用《櫻桃小丸子》角色及相近視覺。公開發布或商業使用可能涉及著作權與商標授權，建議只作私人邀請用途。

