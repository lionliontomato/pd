# 🍮 布丁の小天地｜整合版

這個版本使用一個統一入口切換兩個既有網站，並以 iframe 載入原網站，不重新製作或覆寫原本的 HTML、CSS、JavaScript、背景、字體、動畫及功能。

## 整合的網站

- 布丁の歌單：https://lionliontomato.github.io/pudding/
- 拉布布の存鑽與存歌：https://lionliontomato.github.io/pm/

## 保留原本版面與資料

- 兩個頁面直接載入原網站，因此各自的版面、字體、背景、動畫、搜尋及互動功能維持原樣。
- 兩個網站仍各自讀取原本的 Google 試算表，不合併、不搬移，也不修改試算表。
- 存鑽頁面在第一次切換時才載入，避免一開啟整合網站就同時觸發兩邊的資料讀取。
- 右上角「在原網站開啟」可另開目前的原始網站。

## 瀏覽器分頁圖示

- 歌單頁啟用時，使用布丁歌單原本的 🍮 SVG 圖示。
- 存鑽頁啟用時，切換為 pm 原網站的 `favicon.svg`，並提供原網站的 `favicon.png` 作為備援。
- 切換功能時，瀏覽器分頁圖示會跟著切換，不會因 iframe 而消失。

## GitHub Pages 部署

1. 下載 ZIP 並解壓縮。
2. 在 GitHub 建立新的 Repository（建議設為 Public）。
3. 將解壓縮後的 `index.html`、`favicon.svg`、`README.md`、`.nojekyll` 上傳至 Repository 根目錄。
4. 開啟 Repository 的 **Settings → Pages**。
5. 在 **Build and deployment** 選擇 **Deploy from a branch**。
6. Branch 選 `main`，資料夾選 `/(root)`，按 **Save**。
7. 等待 GitHub Pages 部署完成，再用電腦及手機各測試一次兩個切換頁面。

## 注意事項

- 原本的 pudding 與 pm 兩個 GitHub Pages 網站必須持續公開且可正常使用。
- 本整合版不會修改原網站程式碼；原網站日後更新，整合入口載入的內容也會同步更新。
- 若原網站未來設定禁止 iframe 嵌入，整合入口可能無法顯示該頁；可使用右上角「在原網站開啟」連結繼續瀏覽。
- 整合入口的分頁標題固定顯示「布丁の小天地」，切換時會依功能更新標題及 favicon。
