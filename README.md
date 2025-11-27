💻 全分鐘制課堂出勤及遲到時長計算器
這個專案是一個簡單、高效的靜態網站應用程式，旨在幫助學生和教師即時追蹤課程出席狀況。它採用 「全分鐘制時間銀行 (Time Budget)」 邏輯，將遲到和缺席統一轉換為分鐘來計算，確保對課程規定的最大允許缺席額度有最精確的掌握。

✨ 核心功能 (Features)
分鐘優先 (Minute-First Logic): 將所有缺席堂數和遲到分鐘數統一納入一個「時間銀行」進行計算。

預期最終比率 (Projected Rates): 計算學生在該課程中預期能達到的最終最高出席率和總消耗率，以評估是否滿足及格要求（例如：必須達到 80% 出席）。

剩餘緩衝時間 (Remaining Buffer): 清楚顯示尚餘多少分鐘的「缺席額度」，防止因零星遲到而不知不覺超過限制。

即時警告 (Instant Alerts): 當剩餘緩衝時間少於一堂課，或總消耗時間超過上限時，即時發出視覺警告。

跨平台使用 (Cross-Platform): 作為單頁 HTML 檔案，可以在任何現代瀏覽器中運行。

🛠️ 使用方法 (How to Use)
1. 線上使用 (Online Usage - Via GitHub Pages)

如果您已將檔案託管在 GitHub Pages，只需訪問您的專案網址即可：

[https://username.github.io/repository-name/attendance.html](https://username.github.io/repository-name/attendance.html)
2. 本地使用 (Local Usage)

下載專案中的 attendance.html 檔案。

直接用任何網頁瀏覽器（如 Chrome, Edge, Safari）打開該檔案。

輸入您的課程數據，點擊「計算狀態」按鈕即可獲得結果。

📊 關鍵計算邏輯 (Key Calculation Formulae)
本系統的核心是將所有時間折算為分鐘進行比較。

1. 總允許缺席時間 (Maximum Allowed Time)

這是課程規定允許缺席的總時長。

T 
Max
​	
 =T 
Course
​	
 ×R 
MaxAbs
​	
 
2. 總消耗時間 (Total Consumed Time)

這是學生目前因缺席或遲到而累積消耗的總時長。

T 
Consumed
​	
 =(N 
Abs
​	
 ×T 
Duration
​	
 )+T 
Lateness
​	
 
3. 預期最終出席率 (Projected Final Attendance Rate)

這是假設學生不再缺課/遲到的情況下，最終成績單上能達到的最高出席百分比。

R 
Att
​	
 =100%−( 
T 
Course
​	
 
T 
Consumed
​	
 
​	
 ×100%)