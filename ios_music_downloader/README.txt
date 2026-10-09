iOS 音樂下載器（Safari 網頁 App）
=================================

檔案：
- index.html：完整網頁程式
- manifest.webmanifest：主畫面網頁 App 設定
- icon.svg：圖示

部署方式（GitHub Pages）：
1. 登入 GitHub，建立新的 Public repository，例如 ios-music-downloader。
2. 在 repository 選 Add file > Upload files，上傳以上三個檔案。
3. Commit changes。
4. 進入 Settings > Pages。
5. 在 Build and deployment 選 Deploy from a branch。
6. Branch 選 main，資料夾選 /(root)，按 Save。
7. 等待網站部署完成，開啟 GitHub Pages 顯示的網址。

加入 iPhone 主畫面：
1. 用 iPhone 的 Safari 開啟網站網址。
2. 點分享按鈕（方框向上箭頭）。
3. 選「加入主畫面」（若有「以網頁 App 開啟」選項，可依需要啟用）。
4. 點「加入」。

使用方式：
- 網址下載：貼上可直接存取的音訊檔案網址，按「下載音訊」。
- 如果因 CORS 或網站限制而失敗，按「開啟網址」，再用網站本身的下載/分享功能。
- 匯入檔案：按「選擇『檔案』中的音樂」，從 iOS 檔案選擇器挑選。
- 下載到 iPhone：Safari 對下載的處理方式依 iOS 版本而異，必要時用分享選單的「儲存到檔案」。

限制：
- 靜態網頁無法繞過 CORS、登入、DRM 或網站下載限制。
- 從「檔案」選取的音樂不會被網頁自動搬移；只在頁面工作期間可用。
- iOS 可能不允許網頁在背景持續下載；暫停/續傳不是所有來源都支援。
- 本機紀錄存在瀏覽器 localStorage，清除網站資料可能會刪除紀錄。
