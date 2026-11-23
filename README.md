# 排程表 Beta

免註冊、資料只存在您自己裝置上的排程表。排人、排課、排事情都可以。

A free, sign-up-free scheduler that keeps all your data on your own device. Works for staff shifts, lessons, and everyday plans.

---

## 中文

### 這是什麼
一個打開就能用的排程工具。理髮師記客人時段、音樂老師排課、小團隊排班、家裡排接送都適用。排進去之前就會告訴你有沒有撞期。

### 主要功能
- **日／週／月檢視**，參考 Outlook 的版面
- **點一下就排、拖一下就改**，拉底部可以改長短
- **撞期提醒**：同一個人或同一個地點同時被排兩件才算撞，撞到時先警告再確認，也能一鍵改到最近的空檔
- **交換時段**：兩筆互換時間，換了會撞的先標紅
- **展延該時段**：固定的課或班一次延一個月到六個月，撞到的那週自動跳過
- **異動通知**：改時間、交換、取消之後，一鍵複製通知文字，貼到 LINE 傳給對方
- **加到手機行事曆**：開始前 30 分鐘由手機提醒你

### 隱私
- 所有排程只存在你這台裝置（手機、平板或電腦）的瀏覽器裡，**不會上傳到任何伺服器**
- 手機和電腦的資料各自獨立、不會互通，要用備份檔搬過去
- 這個網站只負責把工具送到你的裝置，收不到、也看不到任何人的資料
- 沒有帳號、沒有追蹤、沒有廣告
- 可設定 4～8 位數字密碼鎖
- 備份檔用你設定的密碼加密（AES-256），沒有密碼打不開

### 開始使用
1. 用手機或電腦打開網址
2. **iPhone**：Safari 下方「分享」→「加入主畫面」
   **Android**：Chrome 會跳出「安裝」，或從選單選「安裝應用程式」
3. 之後從主畫面打開，沒網路也能用

### 換手機或電腦
舊裝置：「設定與備份」→「匯出加密備份」→ 存到雲端硬碟或用 LINE 傳給自己
新裝置：「設定與備份」→「匯入備份」→ 選檔案、輸入密碼

### 常見問題
**資料會不見嗎？** 清除瀏覽器資料、或 iPhone 上很久沒打開，資料可能會被系統清掉。請加到主畫面，並定期匯出備份（超過 30 天沒備份會提醒你）。
**忘記密碼鎖怎麼辦？** 密碼無法找回，只能清除資料重來，再用備份檔還原。
**要錢嗎？** 不用。

### 意見回饋
這是試用版，按頁面上方的「💬 意見回饋」，複製問卷填好後傳給分享連結給你的人。

---

## English

### What it is
A scheduler you can use right away, no account needed. Barbers, music teachers, small teams, and families can all use it. It warns you about conflicts before you save.

### Features
- Day / week / month views (Outlook-style layout)
- Tap to add, drag to move, drag the bottom edge to resize
- Conflict check by person or place, with a one-tap "move to the next free slot"
- Swap two time slots (conflicting candidates are flagged first)
- Extend a recurring slot for one to six months, skipping weeks that clash
- One-tap change / cancellation notices to paste into LINE or any chat app
- Add any slot to your phone's calendar with a 30-minute reminder

### Privacy
- All data stays in the browser on your device (phone, tablet, or computer). Devices don't sync with each other; use a backup file to move data. Nothing is uploaded.
- The website only delivers the app. It cannot receive or see anyone's data.
- No accounts, no tracking, no ads.
- Optional 4–8 digit PIN lock.
- Backup files are encrypted (AES-256) with a password you choose.

### Install
Open the link on your phone. iPhone: Safari → Share → Add to Home Screen. Android: tap "Install" in Chrome. It works offline after that.

### Switching devices
Old device: Settings & backup → Export encrypted backup. New device: Import backup, then enter the password.

---

## 給維護者 / For maintainers
- 純前端單一頁面：`index.html` + `manifest.webmanifest` + `sw.js` + 圖示
- 放上 GitHub Pages：把這個資料夾的檔案上傳到 repository 根目錄 → Settings → Pages → Branch 選 `main` → Save
- **更新網站時**，請把 `sw.js` 第一行的版本號改掉（例如 `paicheng-beta-0.9.1`），使用者才會看到「有新版本」
- `index.html` 已加上 `noindex`，不會被搜尋引擎收錄；想公開時刪掉 `<meta name="robots" ...>` 那一行

授權 License：MIT
